---
title: Sample Presentation
subtitle: Presentations with Pandoc & Reveal.js
author: The Author
date: 31 Jul 2023
---

# Overview

- Introduction
- Methods
- Results
- Conclusion


# Results

## Images

![](images/presentation.svg){.r-stretch .r-frame}

The `r-stretch` class resizes an image to use the remaining space (see [reveal.js layout](https://revealjs.com/layout/)).

---

:::{.r-fit-text}
Or some text.
:::

---

With horizontal lines (`---` in Markdown), a new slide can be started without a heading.


## Fragments

Fragments can be used to reveal parts of a slide gradually (see [reveal.js fragments](https://revealjs.com/fragments/)):

:::{.r-stack .r-stretch}

![](images/presentation.svg){.fragment .fade-out}

:::{.incremental}
- Revealing bullet points
- one by one
- is also possible.
:::

:::

## Background Images {background-image="images/presentation.svg"}


# Conclusion

## Good luck!
