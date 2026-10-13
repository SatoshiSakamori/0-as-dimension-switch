# Zero as a Dimension Switch

**Status: Phase 1 — signed logarithmic coordinates with a shared zero boundary.**

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

Approaching zero from positive or negative values gives two labelled approaches. **We now identify the limiting boundary for both branches as one shared state**, written \(0_\partial\) (Section 3). It has no sign of its own; no physical reflection or new arithmetic rule is assumed.

## 2. Arithmetic and exact cancellation

Multiplication and division of nonzero values become

\[
(s,u)\odot(t,v)=(st,u+v),\qquad
(s,u)\oslash(t,v)=(st,u-v).
\]

Sign reversal is \(N(s,u)=(-s,u)\). It is not motion across a boundary.

**Addition inside the nonzero domain alone is partial.** Put \(M=\max(u,v)\) and \(m=\min(u,v)\).

- If the signs agree, the result is \((s,M+\ln(1+e^{m-M}))\).
- If the signs differ and \(u\ne v\), the result has the sign of the operand with larger \(u\), with log-magnitude \(M+\ln(1-e^{m-M})\).
- If the signs differ and \(u=v\), the ordinary sum is **exactly zero**, so there is no output inside \(\mathcal S^*\).

In particular, \(1+(-1)=0\) cannot be completed **inside \(\mathcal S^*\) alone**. The next section adds a shared boundary and defines continued calculation. Doing so with unchanged arithmetic reconstructs the real numbers.

## 3. Shared zero boundary: ordinary arithmetic continues

Add a single element for zero, shared by the positive and negative branches:

\[
\overline{\mathcal S}=\mathcal S^*\sqcup\{0_\partial\},\qquad
\widehat\Phi(s,u)=s e^u,\quad\widehat\Phi(0_\partial)=0.
\]

This boundary is **not a finite signed-log pair**. On either branch, \(u\to-\infty\) corresponds to approaching it. The extension \(\widehat\Phi\) is a bijection onto the real numbers.

We explicitly keep **the same addition and multiplication rules as the real numbers**:

\[
a\boxplus b=\widehat\Phi^{-1}\bigl(\widehat\Phi(a)+\widehat\Phi(b)\bigr),
\qquad
a\boxtimes b=\widehat\Phi^{-1}\bigl(\widehat\Phi(a)\widehat\Phi(b)\bigr).
\]

Subtraction means adding the sign-reversed operand. Division is defined only for a **nonzero divisor**. A calculation may yield \(0_\partial\) through exact cancellation, and arithmetic can then continue:

\[
(+1,0)\boxplus(-1,0)=0_\partial,\qquad
0_\partial\boxplus(-1,0)=(-1,0),
\]

\[
(+1,0)\boxplus(-1,\ln 2)=(-1,0).
\]

The last example is **\(1-2=-1\)**: magnitude 1 is now on the negative-sign branch. At the shared boundary, adding a positive value enters the positive branch and adding a negative value enters the negative branch. There is no physical bounce and no additional choice of direction.

The distance \(d(a,b)=|\widehat\Phi(a)-\widehat\Phi(b)|\) makes both branches converge to the **same boundary**. A finite log-coordinate never equals \(-\infty\); exact cancellation instead produces the boundary element directly as the result of an operation.

**Key mathematical conclusion:** The extended arithmetic is **isomorphic to ordinary real arithmetic**. Although \(0_\partial\) is not a finite coordinate pair, it *is* an element of the extended algebra: it remains the additive identity, multiplication by it still gives zero, and division by it is undefined. Calling zero a boundary is a representation, not a proof that zero is intrinsically nonnumeric or that singularities disappear.

## 4. Limits and singularities

Reciprocal inversion maps \((s,u)\) to \((s,-u)\). As \(x\to0\) and \(u\to-\infty\), the reciprocal log-magnitude diverges to \(+\infty\). **The singular behavior has not disappeared.** Nor has division by zero become defined.

Likewise, genuinely different limits from the positive and negative sides remain different. Separate sign branches make that distinction explicit; they do not eliminate its mathematical necessity.

A change of coordinates may remove some *coordinate-dependent* singularities, but cannot alone fix an intrinsic divergence of a physical quantity. The claim that zero causes physical singularities would require an independent physical argument.

This sign-plus-logarithm encoding is closely related to the known **signed logarithmic number system (LNS)**. Phase 1 uses established mathematics. The title's "dimension" is only a metaphor for a sign-state branch, **not** a spatial dimension.

## 5. Remaining research questions

**Settled here:** Both sign branches meet at one shared zero boundary; subsequent operations follow the **same rules**, with no special memory or changed laws in the mirror branch.

The remaining question is whether these coordinates and boundary descriptions provide a useful perspective on **specific** singularities. Adding memory, alternative boundary rules, or new physics would be a separate hypothesis, not part of this phase.

## Documentation and background

- [Mathematical note (LaTeX)](docs/zero-dimension-switch.tex) — full definitions and limitations.
- The earlier PDF was removed from the current branch because it contained superseded claims. Generate a fresh PDF from the LaTeX source with **pdflatex** in the **docs/** directory.
- [Universal Numbers: Logarithmic Number System](https://stillwater-sc.github.io/universal/number-systems/lns/)
- [XLNS Research: Introduction to LNS](https://github.com/xlnsresearch/xlns/blob/main/LNS_Intro.md)

## Attribution

Initial conceptual motivation: Satoshi Sakamori. Earlier drafts and this revision used language-model assistance; mathematical facts and untested hypotheses are explicitly separated.
