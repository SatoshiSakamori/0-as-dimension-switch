# 🔧 1. Formalizing Zero as a Dimension Switch

## 📘 Premise

In this system, zero (`0`) is **not the center of the number line**, but a **switch point** or **boundary between two spaces**.

We define:

- `ℝ⁺`: the **positive space**, containing numbers like `1`, `2`, ...
- `ℝ⁻`: the **negative space**, not simply "negative numbers" but a **mirror dimension** across zero, with its own elements like `𝟙⁻`, `𝟚⁻`, etc.
- `0`: a **non-numerical switching point** between these two spaces

This approach **preserves the minus operator (`-`)** in its conventional usage (e.g., subtraction), but **redefines negative numbers** like `-1` as distinct symbolic elements such as `𝟙⁻`, which belong to a separate space.

---

## 🧭 Spatial Structure

$$
ℝ = ℝ⁺ ∪ \{0\} ∪ ℝ⁻
$$

- `1 ∈ ℝ⁺` (standard real numbers)
- `𝟙⁻ ∈ ℝ⁻` (mirrored-space element, not a negative number)
- The minus sign (`−`) remains as a **binary operator**, e.g., `a − b`

### Space Membership:

| Space     | Example Elements | Meaning                                |
|-----------|------------------|----------------------------------------|
| ℝ⁺        | `1`, `2`, `π`     | Ordinary real numbers                  |
| ℝ⁻        | `𝟙⁻`, `𝟚⁻`, `π⁻`   | Mirror counterparts across 0          |
| `{0}`     | `0`               | Non-numeric boundary; switch point     |

---

## 🔁 Transformations Between Spaces

We define a transformation `T` that switches between these two spaces:

- Forward:  
  $$ T(a) = a⁻ $$
  Example: `T(1) = 𝟙⁻`

- Inverse:  
  $$ T^{-1}(𝟙⁻) = 1 $$

> These are **not** arithmetic inverses. They are **spatial translations** through the zero switch.

---

## 🌀 Behavior Near Zero

Zero is not a limit point of continuity between the two spaces. That is:

$$
\lim_{x \to 0^+} f(x) \neq \lim_{x \to 0^-} f(x)
$$

Each limit is taken in a different space, with no requirement that they match.

This allows us to handle divergence or singularity near zero (e.g., `1/x`) by recognizing the left and right behaviors as belonging to **incompatible dimensions**.

---

## 📌 Summary Table

| Concept              | Role or Redefinition                                          |
|----------------------|---------------------------------------------------------------|
| `0`                  | Dimension-switch; not a numeric value                         |
| `𝟙⁻`, `𝟚⁻`           | Mirror-space elements in `ℝ⁻`                                 |
| `−` (operator)       | Preserved as traditional subtraction                          |
| `a − b`              | Valid within the same space                                   |
| `T(a)`               | Space translation from `ℝ⁺` to `ℝ⁻`                           |
| `T⁻¹(a⁻)`            | Reverse translation from `ℝ⁻` to `ℝ⁺`                         |
| `a / 0` (future)     | Not undefined — reinterpreted as a **space-jump**             |

---

## 🚧 Notes

This document is part of a broader mathematical exploration into redefining zero and negative values. It is not a finalized theory but a conceptual framework under construction.

The author is a native Japanese speaker and uses tools like **ChatGPT** to clarify structure and phrasing in English. Contributions or suggestions are welcome!
