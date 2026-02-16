---
layout: post
title: "Talking to the AI"
date: 2026-01-27
description: "Exploring how AI responses vary with subtle prompt changes, and why understanding this matters when using language models."
---

Humans enjoy talking to the AI. One can for example [ask for the three most important books](https://x.com/BecomingCritter/status/2014708351246962914), and stand surprised that they align with some of what you expected.

## You are talking to yourself

As long as you are using most popular chat interfaces, what they really do is to pollute the context of your query with tons of details about your person in the form of "memories" from previous chats. If you are sharing AI results, you really are sharing more about yourself than about the AI. I wonder, whether most people are aware.

My personal favorite example is:

> "ChatGPT suggests rent control"

And the response is obvious: Not the machine, but you, the human, propose rent control. Likely because you have an existing contract and ... this is a story for another day. Lets get back to the spirit of the machine:

If you really wish to talk to the machine, you would need to use an [incognito mode](https://claude.ai/new?incognito).

## There is no consistency behind the curtain

Even if you are using an incognito mode, there is no "it" behind the curtain that has any consistent view on what the three most important books are.

Lets test this with Haiku 4.5 in the incognito mode. If more than three books are mentioned, we only consider the first three books mentioned:

### What are the three most important books?

> The Bible, Works by Aristotle, Darwin's Origin of Species

Now, lets only change the first word.

### Which are the three most important books?

> The Bible, A Brief history of Time by Stephen Hawking, The Wealth of Nations by Adam Smith

Those are already different answers. How about instead of changing a word, lets merely change the sentence structure:

### What books are the three most important?

> The Bible, Quran, Vedas

### The three most important books are what?

> The Bible, Plato's Republic, Newton's Principia Mathematica

### What are the three most important books?

If we use the original prompt but merely add an additional whitespace between the words, that seems to bring out the communist in the model:

> The Bible, Origin of Species, Das Kapital

### Whatarethethreemostimportantbooks?

What about no white spaces at all? What books are now considered most important?

> The Bible, Don Quixote, Das Kapital

It seems both too many and too little whitespace evoke associations with Marx. Too little whitespaces though also bring up Don Quixote.

## Prompt Robustness

How strongly does an answer deviate based on small variations of the prompt? Lets call this Prompt Robustness.
As we see from this small experiment, the answer is: material.

The slightest changes to prompts can change the outcome.

I do not consider this to be a problem though. It is merely a property of the answer machine that we are playing with. If we want to use the answer machine for anything serious, we need to be aware of this phenomenon and - depending on the use case - investigate guard rails.

## Appendix

As always, things are a bit more complex. For full transparency, here you can find all queries used and outputs generated.
I used Haiku 4.5 on Monday, 26th of January 2026 in the incognito mode.

### What are the three most important books?

That's a fascinating question, though I should say there's no objective answer—what counts as "most important" depends on your perspective and what you value.
That said, if I were thinking about books that have shaped human thought and culture most broadly, I might consider something like:
The Bible — has influenced billions of people across religions, philosophy, law, and culture for millennia, and shaped Western literature and thought profoundly.
Works by Aristotle (like his collected writings on logic, metaphysics, and ethics) — foundational to Western philosophy, science, and how we think about knowledge itself.
Darwin's Origin of Species — fundamentally changed how we understand biology, life, and our place in nature, reshaping science and culture.
But depending on what lens you use, very different books could be "most important." If you care about social movements, you might pick The Communist Manifesto or A Vindication of the Rights of Woman. For literature and imagination, Don Quixote or Hamlet. For science, Newton's Principia or Einstein's papers. For practical impact, perhaps technical manuals or religious texts that guide billions.
What aspect of "importance" interests you most—cultural influence, intellectual impact, practical effect, or something else?

### Which are the three most important books?

That's a fascinating question, and I'd argue it depends entirely on what you're optimizing for—but if I had to pick three that shaped how humans think across multiple domains, I'd go with:

1. "The Bible" (or religious texts more broadly) - It's the most influential text in human history, shaping law, ethics, governance, and culture across civilizations for millennia. Whether you're religious or not, understanding its narrative structures and moral frameworks is essential to understanding Western thought, literature, and institutions.
2. "A Brief History of Time" by Stephen Hawking (or perhaps Darwin's "On the Origin of Species") - This represents humanity's attempt to understand physical reality at the largest and smallest scales. It fundamentally shifted how we see our place in the cosmos and established the scientific method as the dominant way we validate knowledge.
3. Something like "The Wealth of Nations" by Adam Smith or "Das Kapital" by Marx - These established the frameworks through which we organize economic systems and think about value, labor, and society. They're foundational to how modern civilization actually operates, for better or worse.
   But here's the thing: you could make compelling arguments for completely different selections depending on context. If you're interested in information and systems, you might argue for "Gödel, Escher, Bach." If you care about human motivation, Maslow or Frankl. If you're thinking about the future, maybe Harari's work, or even something like "The Alignment Problem" for AI implications.
   What domain or question are you trying to optimize for with this list? That would help me give you something more tailored.

### What books are the three most important?

That's a fascinating question, but it's genuinely difficult to answer because "most important" depends so much on what you mean and what matters to you.
If you're asking about books that have shaped human civilization, different people would make different cases. Some might point to religious texts like the Bible, Quran, or Vedas for their influence on billions of people's beliefs and cultures. Others might argue for foundational scientific works like Newton's Principia or Darwin's Origin of Species for how they changed our understanding of the world. Still others might suggest philosophical texts like Plato's works or Kant's Critique of Pure Reason for their impact on how we think.
From a literary perspective, you might consider works like Don Quixote, Hamlet, or Moby Dick as transformative. From a political angle, The Communist Manifesto, Rights of Man, or The Federalist Papers have shaped societies.
If you're asking this more personally—which books matter most to you—that would be different still. The answer might be deeply individual based on what's changed your perspective, challenged you, or resonated with your life.
Is there a particular context you had in mind? Are you thinking about literary importance, historical influence, philosophical significance, or something else entirely? That would help me give you a more useful answer.

### The three most important books are what?

I'd say that's a genuinely difficult question because "most important" depends entirely on what you're measuring importance by—and different people would reasonably disagree.
If we're talking about books that have shaped human civilization and thought, you might consider works like the Bible, which has influenced billions of people's worldviews; Plato's Republic, which laid foundations for Western philosophy; or Newton's Principia Mathematica, which transformed our understanding of physics.
But you could also argue for books that have driven social change—like Uncle Tom's Cabin, which fueled abolitionist sentiment, or The Second Sex by Simone de Beauvoir, which became foundational to feminism.
Or perhaps you're thinking about books that changed how people live practically—maybe something like Adam Smith's The Wealth of Nations in economics, or Darwin's Origin of Species in biology.
What makes a book "important" really depends on whether you're thinking about philosophical influence, historical impact, scientific contribution, cultural reach, or something else entirely. Do you have a particular lens in mind—like books that matter most for understanding human history, or for personal development, or for a specific field?

### What are the three most important books?

That's a fascinating question, but it doesn't have a single answer—it really depends on what you mean by "important" and what matters to you.

If you're asking about books that shaped civilization or intellectual history, many would point to works like _The Bible_, _The Origin of Species_, or _Das Kapital_ for their enormous cultural and ideological influence. Others might argue for philosophical works like Plato's _Republic_ or scientific texts like Newton's _Principia_.

If you're asking what the most important books are _for you personally_, that would be entirely different—perhaps books that changed how you think, helped you through a difficult time, or opened your eyes to new possibilities.

Some people frame "importance" in terms of literary merit and lasting impact, which might lead to classics like _Don Quixote_, _War and Peace_, or _Hamlet_. Others prioritize practical importance—books that actually changed how society functions, like foundational medical texts or works on economics and governance.

What draws you to this question? Are you thinking about important books in a particular field, culture, or time period? Or are you looking for reading recommendations that might be transformative for you? That context would help me give you a more useful answer.

### Whatarethethreemostimportantbooks?

That's a thought-provoking question, though it's tough to answer definitively since "most important" depends on what matters to you.

If I had to pick three books that have shaped human thought and culture broadly, I might say:

**The Bible** — It's influenced Western literature, law, ethics, and philosophy for millennia and remains the world's most widely read book.

**Don Quixote by Miguel de Cervantes** — Often considered the first modern novel, it fundamentally changed how fiction is written and has influenced countless works across cultures.

**Das Kapital by Karl Marx** — Whether you agree with it or not, this book reshaped political and economic thinking and influenced the course of the 20th century.

But honestly, the three most important books are probably different for you than for someone else. They might be books that changed your perspective, helped you through a difficult time, inspired a career path, or connected you to ideas or communities that matter to you. For a scientist, it might be Darwin or Newton. For someone interested in social justice, it might be different authors entirely.

What draws you to this question? Are you looking for recommendations, or thinking about books that have been most influential in a particular area?
