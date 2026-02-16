---
layout: post
title: "Hands-Off Coding"
date: 2026-02-14
description: "Software engineer economics are broken. Everything will change. Here is what changed for me so far."
---

TLDR: Software engineer economics are broken. Everything will change. Here is what changed for me so far. Feel free to use [my resources](https://github.com/nikolasrieble/opencode-config) for your own workflow.

## The bitter lesson

Let's start with the obvious, the bitter lesson. Models scale with compute. My brain does not. Almost all of my current work will be done by agents soon. Resistance is futile, let's tackle the challenge.

## Key Learnings

The way I work changed drastically over the last 4 weeks.

### Architectural Exploration at scale

Because the marginal cost of implementation goes to 0, iterating through multiple patterns and designs of implementation is trivial. Previously deadlines would require engineers to make pragmatic compromises in quality - which is just fancy words for landing in a local optimum. You implement something, test it, and then refine it a tad.

Now, redoing the changeset with a different paradigm takes mere minutes.

### Diligence Paradox

Instead of using agents to produce slop, you can use agents to prevent slop. Using agents to challenge the implementation design and testing strategy is trivial.

Importantly, I can scale my own review process across the teams, using my agents for reviewing every PR.

### Human reviewers

Yet they are needed. Not because agents could not do it better - but simply because of inertia and change resistance. Compliance with customer regulations might require human reviewers.

So, for now, let's use agents to prepare PRs for humans. Splitting up PRs by seams into pre-factoring and cleanup PRs is now easier than ever. Takes a few minutes.

Reviewing a changeset and adding comments on the PR for every non-obvious design decision that might otherwise be overlooked in the line-by-line human review - trivial.

## Repeatable patterns

The exciting question is not how to do things, but how to help others repeat what works well. This is an exciting adventure, and we will all be better off by sharing what works well.

### OpenCode

To decouple my own workflow and setup from the provider race to the best model, I choose to use [OpenCode](https://opencode.ai/docs), a provider agnostic tool.

My core insights so far are:

- Context pollution is bad
  - Skills are [unreliable](https://vercel.com/blog/agents-md-outperforms-skills-in-our-agent-evals) and pollute context (even if only their description)
  - MCPs pollute context
- Agents can encapsulate MCPs and skills like prompts and be invoked reliably
- Subagents make all the difference (clear context separation for different concerns)

With that, my current workflow is fully based on agents, and I only use MCPs encapsulated by agents to isolate the MCP usage for the specific use case.

The three most effective agents so far for me are:

### design-ousterhout

This [agent](https://github.com/nikolasrieble/opencode-config/blob/main/agents/design-ousterhout.md) reviews code through [Ousterhout's A Philosophy of Software Design](https://www.amazon.de/Philosophy-Software-Design-2nd/dp/173210221X).

The core idea is simple: The best guard rails for agents is the existing code and established patterns. That means we should evaluate the patterns we establish ourselves. Ousterhout gets it done.

### testing-khorikov

The [agent](https://github.com/nikolasrieble/opencode-config/blob/main/agents/testing-khorikov.md) reviews code through the lense of [Khorikov's Unit testing](https://www.amazon.de/-/en/Unit-Testing-Principles-Automation-Integration/dp/1617296279).

This has been a game changer for agents writing tests. Most of the tests the agents would write were redundant, and testing implementation detail. Over time, such test suites prevent iteration and do not capture regression. Instead, tests should test behavior. Trivial ideas, sure. But Khorikovs analysis provides vocabulary and criteria for evaluation.

### human-review

My fellow humans are tired of PRs coming in at maximum velocity. We must take account for that, and help ease review at our best ability. This [agent](https://github.com/nikolasrieble/opencode-config/blob/main/agents/human-review.md) focuses solely on PR summary, PR size, and explaining design decisions.
