# 🧠 Zero as a Dimension Switch

## Overview

In standard mathematics, the number line is a single continuous axis stretching from negative infinity to positive infinity. **Zero** sits in the middle.

**This project proposes an alternative framework:**

> **Treat 0 not as a number within a line, but as a "Switch" or "Mirror" between two separate positive spaces.**

Instead of passing *through* zero into negative numbers, values **reflect** off zero and enter a **Mirror Space**. This creates a V-shaped or folded number system, conceptually similar to 1D polar coordinates or signed magnitude representation.

---

## Core Concept: The "Bounce" Mechanism

In this framework, there are no "negative numbers" in the traditional sense. Instead, there are **Positive Numbers** and **Mirror Numbers**.

* **Positive Space ($\mathbb{R}^+$):** Standard values (e.g., $1, 2, 3...$)
* **Mirror Space ($\mathbb{R}^-$):** Reflected values (e.g., $1^-, 2^-, 3^-...$)
* **Zero (0):** The **Boundary** or **Gateway** connecting the two spaces.

### Visualizing the Difference

**Standard Number Line:**
Values pass through 0 linearly.
`... <--- (-2) --- (-1) --- 0 --- (1) --- (2) ---> ...`

**Dimension Switch Model (V-Shape):**
Values bounce at 0.
```text
   Mirror Space (R⁻)          Positive Space (R⁺)
         2⁻                         2
          \                        /
           1⁻                     1
             \                   /
              \                 /
               \               /
                -----> 0 <-----
                  (The Switch)

---

## How Calculation Works

When an operation crosses 0, the "Dimension Switch" is triggered. The remaining magnitude is conserved but transferred to the opposite space.

### Example: Subtraction ($1 - 3$)

In standard math, $1 - 3 = -2$.
In this framework, we interpret subtraction as movement towards the origin.

1.  **Start:** At **1** in Positive Space.
2.  **Move:** Subtract 1 to reach **0** (The Switch).
3.  **Remaining Force:** We still have **2** units of subtraction left.
4.  **Switch:** Since we hit the boundary, we deflect into the **Mirror Space**.
5.  **Result:** **$2^-$** (A magnitude of 2 in the Mirror Space).

### Formalizing the Rule

If we define a value as a pair $(magnitude, space)$, where space is $+1$ or $-1$:

$$
x \ominus y = 
\begin{cases} 
(x - y, +1) & \text{if } x \ge y \quad (\text{Stay in Positive Space}) \\
(y - x, -1) & \text{if } x < y \quad (\text{Switch to Mirror Space})
\end{cases}
$$

This ensures that **magnitude is conserved** across the boundary, behaving like a physical reflection or a billiard ball bouncing off a wall.

---

## Why This Matters

* **Physical Intuition:** Fits physical quantities that cannot be negative (like mass or energy) but can have "opposite direction" or "anti-matter" states.
* **Eliminating "Negative" Ambiguity:** Clearly separates the *magnitude* of a value from its *state/orientation*.
* **Educational Value:** Provides a tangible model for understanding vectors, absolute values, and polar coordinates without assuming a linear number line.

---

## Project Structure

* **docs/** — Formal definitions, axioms, and proofs (LaTeX/PDF).
* **README.md** — Concept overview.

---

## Status

This is an **experimental mathematical framework**.
The goal is to construct a consistent axiomatic system where 0 acts as a non-numeric boundary.

Feedback and contributions are welcome!