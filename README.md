# Zero as a Dimension Switch

**Status: Phase 1 — an exploratory model using signed logarithmic coordinates.**

## Motivation

The motivating question is whether **zero can be treated as a boundary outside a domain of ordinary nonzero values**, with positive and negative quantities represented as different states. In usual arithmetic, zero is the identity for addition, absorbs multiplication, and is excluded as a divisor. These properties are consistent mathematics, not contradictions, but they motivate an alternative perspective on boundaries and singularities.

This phase does **not** claim to remove mathematical or physical singularities or establish a new number system. Earlier unsupported descriptions involving a physical bounce, magnitude conservation, antimatter, and phase transitions have been withdrawn.

## 1. The nonzero-value model

Let

\[
\mathcal S^*=\{+1,-1\}\times\mathbb R,\qquad
\Phi(s,u)=s e^u.
\]

Here \(s\) is a **sign state** and \(u=\ln|x|\) is the **log-magnitude coordinate**. The map \(\Phi\) is a bijection between \(\mathcal S^*\) and the nonzero reals \(\mathbb R\setminus\{0\}\).

| Ordinary \(x\) | State \(s\) | Coordinate \(u\) |
| --- | --- | --- |
| \(10\) | \(+1\) | \(\ln 10\) |
| \(1\) | \(+1\) | \(0\) |
| \(0.01\) | \(+1\) | \(\ln 0.01\) |
| \(-0.01\) | \(-1\) | \(\ln 0.01\) |
| \(-1\) | \(-1\) | \(0\) |

On either fixed-sign branch, \(x\to0\) corresponds to \(u\to-\infty\). Thus **zero is not an element of** \(\mathcal S^*\). The infinite end is a limit, not a finite number. Note that \(u=0\) and negative values of \(u\) are allowed: they are coordinates, not the original value \(x\).

Approaching zero from positive or negative values gives two labelled approaches. Whether to identify those ends, keep them separate, or define a transition is **still open**. No crossing/reflection dynamics are defined here.

## 2. Arithmetic and exact cancellation

Multiplication and division of nonzero values become

\[
(s,u)\odot(t,v)=(st,u+v),\qquad
(s,u)\oslash(t,v)=(st,u-v).
\]

Sign reversal is \(N(s,u)=(-s,u)\). It is not motion across a boundary.

**Addition is partial.** Put \(M=\max(u,v)\) and \(m=\min(u,v)\).

- If the signs agree, the result is \((s,M+\ln(1+e^{m-M}))\).
- If the signs differ and \(u\ne v\), the result has the sign of the operand with larger \(u\), with log-magnitude \(M+\ln(1-e^{m-M})\).
- If the signs differ and \(u=v\), the ordinary sum is **exactly zero**, so there is no output inside \(\mathcal S^*\).

In particular, \(1+(-1)=0\) cannot be completed in this nonzero domain. One may call exact cancellation a **boundary event**, but doing so does not define arithmetic with that event. If zero is added back and the ordinary operations are retained, the result is merely another representation of the real numbers.

## 3. Limits and singularities

Reciprocal inversion maps \((s,u)\) to \((s,-u)\). As \(x\to0\) and \(u\to-\infty\), the reciprocal log-magnitude diverges to \(+\infty\). **The singular behavior has not disappeared.** Nor has division by zero become defined.

Likewise, genuinely different limits from the positive and negative sides remain different. Separate sign branches make that distinction explicit; they do not eliminate its mathematical necessity.

A change of coordinates may remove some *coordinate-dependent* singularities, but cannot alone fix an intrinsic divergence of a physical quantity. The claim that zero causes physical singularities would require an independent physical argument.

This sign-plus-logarithm encoding is closely related to the known **signed logarithmic number system (LNS)**. Phase 1 uses established mathematics. The title's "dimension" is only a metaphor for a sign-state branch, **not** a spatial dimension.

## 4. Future research questions

1. Should zero approaches give two boundary states, one identified boundary, or states retaining a history of approach?
2. Can boundary-event operations and state transitions be defined consistently, including subsequent operations?
3. If a boundary rule changes arithmetic, which familiar algebraic laws survive?
4. In concrete examples, which singularities are coordinate artifacts and which persist?

These questions remain **unanswered**. They are candidates for a later phase, not results of the current model.

## Documentation and background

- [Mathematical note (LaTeX)](docs/zero-dimension-switch.tex) — full definitions and limitations.
- The earlier PDF was removed from the current branch because it contained superseded claims. Generate a fresh PDF from the LaTeX source with **pdflatex** in the **docs/** directory.
- [Universal Numbers: Logarithmic Number System](https://stillwater-sc.github.io/universal/number-systems/lns/)
- [XLNS Research: Introduction to LNS](https://github.com/xlnsresearch/xlns/blob/main/LNS_Intro.md)

## Attribution

Initial conceptual motivation: Satoshi Sakamori. Earlier drafts and this revision used language-model assistance; mathematical facts and untested hypotheses are explicitly separated.
