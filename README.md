# 👣 Project: Step Into the Data – Plantar foot Pressure Analysis for Biomechanics

## Overview

* Investigated how plantar pressure distribution changes across different foot zones under static vs. dynamic conditions.
* Designed as an experimental biomechanics study, showcasing end-to-end statistical analysis.
* Goal: uncover patterns that could inform injury prevention, footwear design, and training practices.


## Methodology

* Data: Plantar pressure recordings segmented into heel, midfoot, forefoot, and toe regions.
* Design: Repeated-measures experiment – same participants tested under multiple conditions.

### Analysis pipeline:

* Descriptive statistics + assumption checks (normality).
* Repeated-measures ANOVA to detect overall differences.
* Post-hoc paired t-tests to identify specific zone/condition effects.
* Tools: Python (pandas, numpy, scipy/statsmodels), matplotlib & seaborn for visualization.

## Results 

* Forefoot: No significant difference between stable and unstable surfaces (Wilcoxon, z = -1.274, p = 0.203) → similar loading across conditions.
* Midfoot: Significant reduction on unstable surface (Paired t-test, t(9) = 5.902, p < 0.001, Cohen’s d = 3.86, huge effect)
* Heel: Significant reduction on unstable surface (Paired t-test, t(9) = 8.201, p < 0.001, Cohen’s d = 7.98, huge effect)
* Lateral foot: Significant reduction on unstable surface (Wilcoxon, z = -2.803, p = 0.005, Cohen’s d = 6.37, huge effect)
* Medial foot: Significant reduction on unstable surface (Wilcoxon, z = -2.497, p = 0.013, Cohen’s d = 4.37, huge effect)
  
### Comparison of Mean Peak Pressure between Stable & Unstable surfaces

![Mean Peak Pressure](visuals/peakpressure.png)

## Key Insights

* Plantar pressure shifted dramatically from heel and midfoot → forefoot on unstable surfaces.
* Large effect sizes confirm these are not trivial differences, but substantial biomechanical shifts.
* Supports the view that unstable surfaces force greater forefoot loading, relevant for injury prevention, footwear design, and performance training.
  


## Key Takeaways

* Demonstrates hypothesis-driven statistical reasoning and rigorous experimental design.
* Strong example of applied data analysis beyond ML (ANOVA, t-tests, assumption checks).
* Highlights ability to derive actionable insights from biomechanical data and communicate them with clear visuals.
