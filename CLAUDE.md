# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

AP Statistics educational materials for teaching sampling and experimental design concepts. Uses the "Three Rivers Problem" scenario where students explore different sampling methods on a 50-plot farm field with a yield gradient (high near river, low near dusty road).

## File Structure

- `three_rivers_worksheet.tex` - LaTeX worksheet covering convenience sampling, SRS, stratified sampling, and blocking for experiments. Includes teacher answer key.
- `poster_a_convenience.html` - Interactive poster demonstrating biased convenience sampling
- `poster_b_srs.html` - Interactive poster demonstrating Simple Random Sample with high variation
- `poster_c_stratified.html` - Interactive poster demonstrating stratified sampling with low variation

## Development

**HTML Posters**: Self-contained single-file web apps with embedded CSS and JavaScript. Open directly in browser - no build step required. Each poster includes interactive sampling generators that students can click to see different random samples.

**LaTeX Worksheet**: Compile with any LaTeX distribution that includes TikZ:
```bash
pdflatex three_rivers_worksheet.tex
```

## Key Data

All materials use the same 50-plot field data:
- Column A (near river): mean = 99.6
- Column B: mean = 79.8
- Column C: mean = 60.2
- Column D: mean = 39.8
- Column E (near road): mean = 19.9
- **True population mean = 59.86**

## Pedagogical Goals

The materials demonstrate:
1. **Bias** - Convenience sampling systematically underestimates (undercoverage)
2. **Variation** - SRS is unbiased but inconsistent; stratified sampling reduces variation
3. **Blocking** - Experimental design parallel to stratification in sampling
