# Dow-Jones-Cycle-Analysis

Rules-based framework for identifying equity index cycles via absolute/relative extrema, implemented in Excel and designed to generalise across markets.

## Overview
This repository contains an Excel workbook that operationalises a simple, event-driven method for segmenting an equity index into alternating bull and bear phases. The approach avoids traditional technical indicators (e.g., moving-average crossovers) and instead defines cycles using unambiguous conditions on *relative* maxima/minima and the resulting *absolute* turning points.

A long-horizon case study is included for the Dow Jones Industrial Average, summarising cycle start/end dates, durations, and percentage moves.

## Repository contents
- `Dow_Jones_104_Cycle_Analysis.xlsx`  
  Main workbook (cycle tables, definitions, and results).
- `cycles/`  
  Visual Chart screenshots illustrating example cycles and annotations.

## Method summary 
1. **Choose a base period** (e.g., monthly) and determine **relative maxima/minima** within each period.
2. Use threshold rules (e.g., **β** and **γ**, defined as percentages of prior extrema) to determine **absolute maxima/minima**.
3. Define bearish/bullish phases via **clearly specified events** (e.g., sequences of lower relative highs or lower relative lows).
4. Produce a cycle table with:
   - Cycle boundary dates (bull start, bull end, bear end)
   - Duration in years (up / down / total)
   - Price levels at boundaries and % moves

## How to use
1. Open `Dow_Jones_104_Cycle_Analysis.xlsx`.
2. Review the cycle definition section (parameters and event conditions).
3. Inspect the cycle table outputs (dates, durations, and % up/down).
4. Optionally, compare the tabulated cycles to the annotated examples in `cycles/`.

## Possible extensions
- Re-implement the methodology in Python for full reproducibility and easier parameter sweeps.
- Extend the case study to additional indices (S&P 500, DAX, Nasdaq 100) and compare cross-market cycle statistics.
