# CV

Clovis SFEIR's CV, written in LaTeX and compiled with [Tectonic](https://tectonic-typesetting.github.io/). One page, kept that way on purpose — every push is checked by CI.

[![Build](https://github.com/sfeirc/CV/actions/workflows/build.yml/badge.svg)](https://github.com/sfeirc/CV/actions/workflows/build.yml)

## Download

[cv.pdf](cv.pdf) — always the latest compiled version.

## Build it yourself

```bash
tectonic cv.tex
```

## Why LaTeX

Precise control over spacing and page count matters more for a CV than it sounds: this one went through several iterations of margin/font tuning to fit everything on exactly one page without cutting content that mattered. CI (`.github/workflows/build.yml`) recompiles `cv.tex` on every push and fails the build if the result is anything other than exactly one page, so that constraint can't silently regress.

## Role-targeted versions

`applications/` holds six archetype variants of this CV — `systems_swe.tex`, `platform_engineer.tex`, `quant_dev_trading.tex`, `market_maker_trader.tex`, `quant_research.tex`, `discretionary_research.tex` — each reasoned independently about which projects actually fit that role family (not just relabeled), reordering the project lineup, profile summary, and skills emphasis, all still one page. `applications/pdf/` has the compiled PDFs, one per Summer 2027 internship application, named by company and role.
