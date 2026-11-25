# copilot-experiment-0003

## Function Plotter

A single-file, dependency-free HTML/JavaScript app (`index.html`) that plots continuous
math functions and their combined (summed) function.

### Usage

Open `index.html` in any modern web browser (no build step or server required).

- **Add function** to add a term, then pick its base function from the dropdown:
  `sin`, `cos`, `tan`, `sinh`, `cosh`, `tanh`, `atan`, `exp`, `ln`, `sqrt`, `|x|`,
  `x`, `x²`, `x³`, `1/x`, `exp(-x²)`, `sinc`.
- Each term is plotted as `A·f(B·x + C) + D` (amplitude, frequency, phase, offset).
- All visible terms are summed and drawn as the thick black **Σ (sum)** curve.
  Uncheck a term to hide it and exclude it from the sum.
- Set the x/y range manually, use **Auto-fit Y**, drag to pan, and scroll to zoom.
- Hover over the plot to read each term's value and the sum at the cursor.
- Discontinuities (e.g. asymptotes of `tan` and `1/x`) and points outside a
  function's domain (e.g. `ln(x)` for `x ≤ 0`) are left as gaps rather than joined.
