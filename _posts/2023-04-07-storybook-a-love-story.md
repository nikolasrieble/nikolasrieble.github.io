---
layout: post
title: "Storybook - A love story"
date: 2023-04-07
summary: "A storybook-first approach improves developer experience, velocity and quality of the codebase."
---

# Storybook - A love story

2023-04-07, Storybook, Tests, React, Recharts, Tulip Interfaces

This is a story about how I fell in love with Storybook. I started using React two years ago when I joined [Tulip Interfaces](https://tulip.co/). We use storybook to document our shared components. A storybook-first approach improves developer experience, velocity and quality of the codebase. I became contributor to [recharts](https://recharts.org/en-US/storybook). Here storybook helps us to ship changes to a complex and popular library with confidence.

## An encapsulated development environment

Storybook is a development environment for UI components. It reloads quickly, and will always be quicker than whichever main application you are developing for. A sandbox where you can develop components in isolation, without the distraction of the rest of the application.

## A living documentation

Addons such as [Docs](https://storybook.js.org/blog/storybook-7-docs/) incentivise developers to write good documentation. Auto generated controls allow easy exploration of the component's API. Because the stories use the source code, they are hardly ever outdated.

## Documentation as tests

With the [storybook test runner](https://storybook.js.org/addons/@storybook/test-runner), all stories are tests. Every story is a test that verifies that the component renders with error. Further, play functions test interactions with user event. Setting up such tests is much easier than unit tests such as with react-testing library.

## Storybook first approach separates component design and integration.

When developing a component, you can focus on the component itself, without worrying about the rest of the application. When integrating the component, you can focus on the integration, without worrying about the component itself. The reduced complexity results in smaller PRs and faster development.

I am all in on storybook. I am convinced that it is the best way to develop UI components.

If you like to work with Storybook, come join us at either Tulip Interfaces, or as a contributor to Recharts.
