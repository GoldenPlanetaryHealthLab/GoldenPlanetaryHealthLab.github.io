---
title: "Environments & Package Management"
format: html
---

## Why this guide exists

One of the most common sources of frustration in scientific computing is **software installation**.

You may have encountered issues like:

- “This package won’t install on the cluster”
- “It works on my laptop but not on FASRC”
- “CMake can’t find a dependency”
- “glibc version is too old”

These are not random errors — they all stem from the same root cause:

::: {.callout-important}
**Software lives at different layers of your system, and not all tools manage the same layer.**
:::

This guide introduces a simple mental model to help you understand:
- where software should be installed
- which tools to use
- how to avoid breaking your environment

---

## The Layered Model

We organize software into **three layers**:

```{mermaid}
flowchart TD
    A[Project Layer<br>Code + Pipelines + Config] --> B[Language Environments<br>uv (Python) / rv (R)]
    B --> C[System Dependencies<br>brew / cargo / webi]

    C --> D[Underlying OS<br>FASRC / macOS / Linux]

    style A fill:#e3f2fd,stroke:#1e88e5
    style B fill:#e8f5e9,stroke:#43a047
    style C fill:#fff3e0,stroke:#fb8c00
    style D fill:#f3e5f5,stroke:#8e24aa