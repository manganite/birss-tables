# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project overview

This is a transcription/digitization project, not a software codebase. The goal is to produce accurate Markdown transcriptions of specific tables and reference material from `Birss Symmetry & Magnetism komplett.pdf` (a crystallography/tensor-physics textbook), which are otherwise hard to read because many tables are printed rotated 90° or split across pages.

## Files

- `Birss Symmetry & Magnetism komplett.pdf` — the source PDF (large, ~24MB). Reference by page number when extracting content.
- `conventions-reference.md` — a compiled glossary of notation conventions used across all tables (axis conventions, Hermann–Mauguin/Schoenflies/Shubnikov notation, generating matrix (σ) notation, tensor component grouping notation like `xxy(3)`, `(c4)`, `(xy:6)`, etc.). **Read this first** before transcribing or interpreting any table — it defines the symbols used consistently across `table-*.md`.
- `table-3.md` — the 32 crystallographic point groups: symmetry operations, generating matrices.
- `table-4a.md` through `table-4f.md` — tensor forms (independent components) for ranks 0–4 across all 32 point groups, keyed by symbols defined relative to Table 4a's symbol-equivalence mapping.
- `table-6.md` — the 122 magnetic point groups.
- `table-7.md` — magnetic point groups mapped to tensor symbols (i-tensors / c-tensors, polar/axial, even/odd rank).
- `.tmp_ocr/` — scratch directory containing cropped page images (`.png`) and raw OCR text dumps (`.txt`) used as intermediate working material while transcribing tables. Treat as disposable working files, not final output.

## Working conventions

- Each `table-N.md` begins with a `Source:` line citing the scanned PDF page numbers (and printed book page numbers where they differ) and any page-rotation/splitting notes.
- Notation choices (overbars written as leading `-`, `⊥` for perpendicular, `//` for parallel axes, `.` as Shubnikov separator, etc.) must stay consistent with `conventions-reference.md`. If a new notation convention is introduced while transcribing a table, add it to `conventions-reference.md` as well.
- When transcribing a new table or fixing an existing one:
  1. Identify the relevant PDF page range and check `.tmp_ocr/` for existing crops/OCR of those pages before re-extracting.
  2. Cross-check transcribed symbols (point group symbols, tensor symbols like `A_m`, `B_n`, generating matrix indices `sigma^(n)`) against `table-3.md` and `table-4a.md`, since these symbols are shared/cross-referenced across tables.
  3. Use `0` for vanishing tensor components and `-` for blank/not-applicable table cells (per existing convention in `table-4a.md`).
- These tables are dense and error-prone to OCR (rotated text, small subscripts, special symbols `⊥ ● ○ –`). When transcribing, prefer cropping/zooming the relevant region of the PDF page over relying on raw whole-page OCR.
