# 🧠 Zero as a Dimension Switch

## Overview

In the usual number line, **0** sits at the center between positive and negative numbers.  
But 0 has unique mathematical properties — division by 0 is undefined, and it is often the source of singularities.  

**This project explores an alternative interpretation:**  
> Treat 0 not as a regular number, but as a **boundary between two separate spaces**.

Inspired by examples like **absolute zero temperature** (where values only exist on one side),  
we propose a framework where **0 is a dimension switch**, allowing us to reinterpret problematic operations such as division by 0.

---

## Core Idea

- **0 is a non-numeric boundary** between two spaces:
  - Positive space: \( \mathbb{R}^+ \)
  - Mirror space: \( \mathbb{R}^- \), with elements like \( 𝟙⁻, 𝟚⁻ \)
- **Negative numbers** are reinterpreted as elements of a mirror dimension, not just values below zero.
- Crossing 0 means applying a **space transformation** \( T \):
  - \( T(a) = a⁻ \)
  - \( T^{-1}(a⁻) = a \)
- No requirement for continuity across 0:
  \[
    \lim_{x \to 0^+} f(x) \neq \lim_{x \to 0^-} f(x)
  \]

---

## Why This Matters

- Avoids certain divergences and singularities by **breaking continuity** across 0.
- Offers a fresh viewpoint for:
  - Functions like \( 1/x \)
  - Physical quantities with one-sided boundaries
  - Geometric and algebraic extensions (projective space, hyperbolic geometry, etc.)

---

## Project Structure

- **docs/** — Formal definitions and symbolic rules (LaTeX → PDF)
- **README.md** — This high-level summary
- Planned:
  - Animated visualizations with Manim
  - Python simulations
  - Extensions to other number systems

---

## Detailed Theory

A complete explanation, with formal notation and examples,  
is available in the LaTeX document here:  
📄 [Zero as a Dimension Switch — Full Paper (PDF)](./docs/zero-dimension-switch.pdf)

---

## Status & Feedback

This is an **experimental mathematical framework** under development.  
Contributions, critiques, and new perspectives are welcome.

---