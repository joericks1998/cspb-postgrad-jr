# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Graduate-level discrete mathematics coursework repository (CSPB - Logic and Reasoning). Contains homework assignments (hw1–hw4) written in LaTeX, covering propositional logic, proof techniques, quantifiers, and formal reasoning. References Kenneth Rosen's discrete mathematics textbook throughout.

## Build Commands

Compile any homework PDF with latexmk:
```bash
cd hw<N> && latexmk -pdf hw<N>.tex
```

Clean build artifacts:
```bash
cd hw<N> && latexmk -C
```

## Repository Structure

- `hw1/` – Logic & Reasoning (truth tables, conditionals, inductive/deductive reasoning)
- `hw2/` – Logical equivalences, De Morgan's laws, quantifiers, bitwise operations
- `hw3/` – Direct proofs, contrapositive, contradiction, biconditional proofs
- `hw4/` – Not yet started (empty skeleton)
- `Proof Sheet - Master.pdf` – Reference document

Each `hw<N>/` directory contains `hw<N>.tex` (source) and `hw<N>.pdf` (compiled output), plus latexmk build artifacts.

## LaTeX Conventions

- Document class: `article`
- Core packages: `amsmath`, `amssymb`, `geometry`, `enumitem`, `graphicx`
- Proofs use tabular layouts with justification in the right column
- `\clearpage` separates major sections
- Each assignment includes an honor statement and self-assessment/reflection sections

## Important Notes

- No `.gitignore` exists; LaTeX build artifacts are tracked in git
- VS Code AI features are intentionally disabled (`.vscode/settings.json`) for academic integrity
