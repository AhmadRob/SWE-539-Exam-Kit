# SWE 539 · Software Metrics notes

Study notes for **SWE 539 Software Metrics** at KFUPM (Dr. Mohammad Alshayeb), written by Ahmed Abualrob.
One self-contained page, in the same style as my ICS 553 notes.

**Live page:** `[https://<your-username>.github.io/SWE-539-Exam-Kit/](https://github.com/AhmadRob/SWE-539-Exam-Kit)` (after you turn on GitHub Pages, see below)

## What is inside

| Section | Content |
|---|---|
| Formula wall | Every formula and counting rule on one table, with which direction is "good" |
| Flashcards | 44 cards with flip, "I know it / Review again", topic filter and a review-only mode (progress is saved in your browser) |
| OO metrics | C&K (WMC, DIT, NOC, CBO, RFC, LCOM) and Li (NAC, NDC, NLM, CMC, CTA, CTM), with the slide examples and a clickable inheritance tree |
| Cohesion family | LCOM1–5, Coh, TCC, LCC, CC on one worked class, plus a calculator that computes all of them for any class you type |
| Package metrics | Package cohesion, Ca, Ce, instability, with the slide diagrams |
| Refactoring | Code smells, clone types, Extract / Inline / Move Method, Replace Temp with Query, Extract Class, smell → refactoring tables |
| Ch 1–3, Empirical | Measurement, representation condition, scale types and meaningfulness, GQM and CMMI, study types, hypotheses, validity threats |
| Practice | 35 questions (mostly calculations) with step-by-step answers |

Works on phones, has light and dark mode, and needs no build step.

## Publish with GitHub Pages

1. Create a new repository and upload `index.html`, `.nojekyll` and this `README.md` to the root of the `main` branch.
2. Open **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose `main` and `/ (root)`, then **Save**.
4. After a minute the page is live at `https://<your-username>.github.io/<repo-name>/`.

To add it to an existing notes repository instead, rename `index.html` (for example `SWE539-Metrics.html`) and link to it from your other pages.

## Sources

Summarised from the SWE 539 lecture slides, which draw on:

- N. Fenton and J. Bieman, *Software Metrics: A Rigorous and Practical Approach* (chapters 1–4)
- S. R. Chidamber and C. F. Kemerer, "A Metrics Suite for Object Oriented Design", IEEE TSE, 1994
- W. Li, "Another metric suite for object-oriented programming", JSS, 1998
- Li & Henry (1993), Hitz & Montazeri (1995), Henderson-Sellers (1996), Briand et al. (1998), Bieman & Kang (1995), Bonja & Kidanmariam (2006), Al Dallal (2011, 2015)
- M. Fowler, *Refactoring: Improving the Design of Existing Code*, 2nd ed., 2018, and refactoring.guru
- R. C. Martin, *Agile Software Development, Principles, Patterns, and Practices*

These are personal study notes, not official course material.

## Notes on two slide values

- **Mean vs median example (Ch 2):** the slide gives mean(Y) = 3.1; the correct value is 23/7 ≈ 3.29. The conclusion does not change.
- **Package cohesion example:** the slide counts 6 relationships among 5 classes (6 / 20 = 0.3). The diagram shows 5 links; the two-way C–D association most likely counts twice because n(n − 1) counts ordered pairs.
