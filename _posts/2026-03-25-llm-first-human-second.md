---
layout: post
title: "Data Visualization: LLM first, human second"
date: 2026-03-25
description: "Interactions happen between agents. Humans are rarely involved."
---

Building for agents and humans.

### Visual comprehension of AI is brittle at best

Models can be fooled by simple things that humans would not even notice, such as shown in [1]. I acknowledge that since then models have improved, the example though is beautifully illustrative.

### Humans need data visualization

For humans on the other side, a boring table of data is not legible. Outliers or other pattern go undetected. Jonathan Schwabisch has written an amazing book on what works well for humans: Charts do. Not pie charts though [2].

### Looking at the problem through the rear mirror

Plenty documents exist that rely on data visualization to convey critical messages, from website over research papers to advertisment. Docling tries to tackle this by extracting data from the visualization [3]

## Take a step back

If we rebuild data visualization tools today, we would build them for agents first, and for humans second. The visualization is a presentation layer.

What does that mean?

### All charts in the web should have a JSON export button.

All charts in Recharts should have a button with which to export a JSON instead. Charts for agents means text. The JSON must include the data.

### You should no longer use any charts. Use JSON and render the chart only for humans.

How you implement the rendering does not matter - as long as the input is JSON. To nobody surprise, Vercel is already working on it [4].

What are the implications? Charts in technical documents should be text. The rendering should be a presentation. Example: Markdown.

Think: Mermaid for charts. In Markdown.

## Prior Art

As always, someone has already spent time here.

### Vega JSON

Vega JSON defines a visualization grammer [5] - and is the perfect candidate for building on top.

### Sources

- [1] [One pixel attack for fooling deep neural networks](https://arxiv.org/abs/1710.08864)
- [2] [Better Data Visualizations: A Guide for Scholars, Researchers, and Wonks](https://www.jstor.org/stable/10.7312/schw19310)
- [3] [Docling Chart Extraction](https://github.com/docling-project/docling/blob/main/docs/examples/chart_extraction.py)
- [4] [Vercel Json renderer](https://github.com/vercel-labs/json-render)
- [5] [Vega JSON](https://vega.github.io/vega/)
