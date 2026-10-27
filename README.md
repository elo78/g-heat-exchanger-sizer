# G-Heat Exchanger Sizer

A browser tool that sizes a heat exchanger using the LMTD method. Enter the hot stream, the cold inlet and U, and it returns the heat duty, cold outlet temperature, LMTD, effectiveness and the area needed.

Live tool: https://elo78.github.io/g-heat-exchanger-sizer

## Method
- Heat duty: Q = m·cp·(Thi − Tho)
- Cold outlet: Tco = Tci + Q / (mc·cpc)
- LMTD = (ΔT1 − ΔT2) / ln(ΔT1 / ΔT2)
- Area: A = Q / (U · LMTD)
- Effectiveness: ε = Q / Qmax

Supports counter-current and parallel flow, and warns on temperature crosses.

## Assumptions
Constant cp and U, no phase change, no heat loss. For shell-and-tube passes, multiply LMTD by a correction factor F.

## Built with
HTML, CSS and JavaScript. No libraries.
