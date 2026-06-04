<div align="center">

# Methods Lab
### Statistical Methods, Made Tangible.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Static Badge](https://img.shields.io/badge/Status-Academic_Project-blue)]()
[![Static Badge](https://img.shields.io/badge/Tech-Vanilla_JS-orange)]()
[![Static Badge](https://img.shields.io/badge/Tools-29_interactive-green)]()

### 🌐 [www.methods-lab.uni-osnabrueck.de](https://methods-lab.uni-osnabrueck.de/)

**A suite of 29 interactive tools that build statistical intuition from the ground up — from OLS regression and effect sizes, through the counter-intuitive paradoxes that trip up even seasoned researchers, into modern causal inference, psychometrics (IRT), and clinical diagnostics. Everything runs entirely in the browser. No code, no server, no data ever leaves your machine.**

[ [Learning Path](#-the-learning-path) ] • [ [Ecosystem](#-the-ecosystem) ] • [ [Philosophy](#-scientific-philosophy) ] • [ [Usage](#-getting-started) ] • [ [Sister Project](#-sister-project--bayes-thinking-lab) ]

---

</div>

> **Language note:** The interface, inline explanations, and help panels are written in **German**, as the lab is used in teaching at the University of Osnabrück. The methods and code are, of course, language-independent.

---

## 🔭 Scientific Philosophy

The **Methods Lab** rejects the "black-box" experience of statistical software, where a number appears and its meaning stays hidden. Instead, every tool makes a concept *manipulable*: move a slider, drag a data point, switch a scenario — and watch the consequence unfold in real time.

* **Regression is the spine.** Almost every method in applied statistics is regression in disguise. The lab is deliberately ordered so that the foundations (Section 1) make the paradoxes (Section 3) and the causal methods (Section 4) feel *obvious in hindsight* rather than mysterious.
* **Paradoxes are not magic.** Berkson, Lord, Simpson, regression to the mean — each becomes transparent once you see the underlying selection or conditioning structure. The lab shows the structure, not just the surprising result.
* **Individual cases, not just group means.** From diagnostic intervals to the Jacobson-Truax method for reliable and clinically significant change, the lab takes seriously the question every practitioner faces: *what does this mean for this one person?*
* **Honest about assumptions.** Tools surface what is usually swept under the rug — non-normal norm samples, measurement error, the arbitrariness of cut-offs, the gap between "reliable" and "meaningful."

---

## 🗺 The Learning Path

The lab is organized into six sections that build on one another. Work through them in order, or jump in wherever your current knowledge begins.

| Section | What you will learn | Key Tools |
| :--- | :--- | :--- |
| **1 · Regression & Relationships** | How linear relationships are estimated and decomposed — the foundation for everything else | OLS Regression · Partial Correlation · Mediation · Moderation · Multilevel Models |
| **2 · Inference & Planning** | How big a sample needs to be, what counts as a meaningful effect, and what missing data does | Effect Sizes · Power & Sample Size · Missing Data |
| **3 · Statistical Paradoxes** | Why counter-intuitive results are, in fact, plain regression logic | Regression to the Mean · Attenuation · Berkson · Lord |
| **4 · Causal Inference** | When association may be read as causation — and the toolkit of modern causal analysis | Causal Foundations · RDD · Difference-in-Differences · Propensity Score Matching |
| **5 · Test Theory & Measurement** | How psychological constructs are measured and how well | IRT (dichotomous & ordinal) · DIF · Factor Analysis · Norm-Score Distortion |
| **6 · Diagnostics & Test Quality** | How accurately an instrument detects what it should — at the level of the individual | Sensitivity/Specificity · ICC · Inter-Rater Agreement · Jacobson-Truax |

---

## 🛠 The Ecosystem

Legend: **✓** finished · **⟳** in revision · **◷** planned

### 1 · Regression & Relationships
*The foundation: how to estimate linear relationships, what "controlling for" means, and how effects split into direct and indirect paths.*

* **✓ OLS & Multiple Regression** — Simple and multiple regression: coefficients, R², assumptions, and typical violations. Interactive data injection.
* **✓ Partial Correlation** — The correlation of two variables purged of a third. Suppressor effects, semi-partial correlation, path coefficients.
* **✓ Mediation Analysis** — Hayes/PROCESS Model 4: DAG visualization, direct and indirect effect, Sobel/Aroian live, bootstrap on demand.
* **✓ Moderation Analysis** — Hayes/PROCESS Model 1: simple slopes, Johnson-Neyman technique, floodlight plot. When does W moderate the effect of X on Y?
* **✓ Multilevel Models** — Complete / no / partial pooling compared, shrinkage caterpillar plot, ICC slider, random slopes (τ₁, ρ), Simpson's paradox experienced live.

### 2 · Inference & Planning
*How large must a sample be? What is a meaningful effect? And what happens when data are missing?*

* **⟳ Effect Sizes** — Cohen's d, r, η², f, OR/RR: conversions, visualizations, confidence intervals. *(NCT confidence-interval computation is currently being reworked.)*
* **✓ Power & Sample Size** — Four-curve family, H₀/H₁ distributions, n×d heatmap, sensitivity curve, MDES, SESOI. α, β, d, n fully interactive.
* **✓ Missing Data** — MCAR, MAR, MNAR: understand the mechanisms, compare four imputation strategies, traffic-light grid for bias and efficiency.

### 3 · Statistical Paradoxes
*Counter-intuitive effects that trap even experienced researchers. All of them rest on regression logic — which is why this section comes after the foundations.*

* **✓ Regression to the Mean** — Blood-pressure example, r-slider, bidirectional selection. Why "bad" extreme values look better the second time.
* **✓ Measurement-Error Attenuation** — Intelligence & school achievement: disattenuation, learning cards on N-instability and reliability choice.
* **✓ Berkson's Paradox** — Talent + effort → success: DAG, diagonal selection boundary, collider bias. Negative correlation in selected samples.
* **✓ Lord's Paradox** — ANCOVA vs. change scores: when do the two analyses lead to opposite conclusions? DAG, key formula, lege-artis decision.
* **◷ Simpson's Paradox** — An aggregate trend reverses on disaggregation; ecological fallacy as a special case. Cross-link to the multilevel tool.
* **◷ Range Restriction** — Taylor-Russell interactive: correlation attenuation in selected samples, Thorndike correction formulae.
* **◷ Lindley's Paradox** — p < .05 yet a Bayes factor < 1 is possible: the frequentist–Bayes conflict. Synergy with the Bayes Thinking Lab.
* **◷ Will Rogers Phenomenon** — Reclassification raises the mean of both groups at once (stage migration). Crucial for longitudinal and staging data.
* **◷ Freedman's Paradox** — Stepwise regression on random predictors: spuriously significant variables, R² inflation. A warning to applied statisticians.
* **◷ Inspection Paradox** — You land by chance in above-average-length intervals (buses, clinical cohorts, survival data). Length-biased sampling.

### 4 · Causal Inference
*Under what conditions may association be read as causation? The potential-outcomes framework, natural experiments, and matching.*

* **✓ Causal Inference — Foundations** — DAGs, potential outcomes, IPW, G-computation: five modules in a full-screen layout. Strong confounding, live ATE estimation.
* **✓ Regression Discontinuity (RDD)** — Sharp RDD: scenarios A–D, polynomial-degree slider, fuzzy RDD, and polynomial pitfalls as expandable modules.
* **✓ Difference-in-Differences** — Regression model, ATT, selection bias, naïve comparisons, live-updating arrows. The parallel-trends assumption made visual.
* **✓ Propensity Score Matching** — Logistic PS estimation, greedy 1:1 matching, IPW (ATT), love plot, estimator comparison before/after matching.

### 5 · Test Theory & Measurement
*How psychological constructs are measured — and how well a test does that.*

* **✓ IRT — Dichotomous Models** — 1PL/2PL/3PL/4PL + Rasch: ICC, TIF, Wright map, MLE person estimation. The Rasch-vs-1PL distinction made explicit.
* **✓ IRT — Ordinal Models** — PCM, GPCM, GRM: CRF, ESC, item information for every item. Disordered-threshold warning, factor-analysis link in the help.
* **✓ Differential Item Functioning (DIF)** — 2PL model, four items, Δb/Δa sliders, ICC comparison, difference curve, group distributions, Raju SA/UA, ETS A/B/C.
* **✓ Factor Analysis** — PAF (genuine EFA), correct oblique solution (pattern matrix Λ), reliability panel (α / ωt / ωh Schmid-Leiman), three scenarios, biplot.
* **✓ Norm-Score Distortion** — What linear T-scores do to right-skewed distributions (SCL-90 analogy). Gamma, log-normal, exponential, Weibull, ex-Gaussian; empirical vs. T-norm percentile ranks; area-transformation (Lienert & Raatz) overlay.
* **◷ Classical Test Theory** — Reliability (α, split-half, test-retest), error variance, SEM, correction for attenuation. Bridge to IRT.

### 6 · Diagnostics & Test Quality
*How well does an instrument detect what it should — at the level of the individual patient?*

* **✓ Sensitivity & Specificity** — ROC curve, AUC, PPV/NPV as a function of prevalence: interactive cut-off, live 2×2 table.
* **✓ Profile Analysis** — Profile comparison with Cattell rₚ, McCrae Iₚₐ/rₚₐ, ICC_de: elevation, scatter, and shape evaluated separately.
* **✓ Test Bias** — Cleary model, Meade & Fetzer, adverse impact: three modules, four scenarios. Differential prediction vs. fairness in practice.
* **✓ ICC-Lab** — Intraclass correlation: all six Shrout-&-Fleiss forms, rater count, absolute vs. consistency agreement.
* **✓ Inter-Rater Agreement** — Cohen's κ, weighted κ, the kappa paradox, prevalence & bias: when κ misleads and what to report instead.
* **✓ Diagnostic Intervals** — Confidence, prediction, and tolerance intervals compared: what each one says and which question it answers.
* **✓ Diagnostic Validity** — Construct, criterion, and content validity: validity coefficients, Taylor-Russell tables, utility analysis.
* **✓ Jacobson-Truax Analysis** — Reliable Change Index & clinical significance: RCI band, cut-off criteria a/b/c/d, five-group classification (analogous to the R package JTRCI) in the pre-post plot. BDI-II and SCL-90 as worked examples.

---

## 🚀 Getting Started

The Methods Lab is a **serverless web application**. No installation, no backend, and no data leaves your machine.

### Option 1 — Use it online (recommended)

Open the hosted version directly in your browser:

🌐 **[www.methods-lab.uni-osnabrueck.de](https://methods-lab.uni-osnabrueck.de/)**

No setup required.

### Option 2 — Run it locally

1. **Clone the repository:**
    ```bash
    git clone https://github.com/raduesing/MethodsLab.git
    ```
2. **Open `index.html`** in any modern web browser.
3. **Follow the learning path** — or jump directly to the tool that matches your current need.

> **Tip:** Every tool includes a built-in **? Help panel** with worked examples, formulae, and references, plus inline explanations for each parameter and a Light/Dark theme toggle.

---

## 🎓 Target Audience

| Level | Recommended Entry Point | Tools to Explore |
| :--- | :--- | :--- |
| **BSc Students** | Section 1 — Foundations | OLS Regression · Partial Correlation · Effect Sizes · Power & Sample Size · Sensitivity/Specificity |
| **MSc Students** | Sections 2–3 | Missing Data · Regression to the Mean · Berkson · Lord · Mediation/Moderation · IRT |
| **PhD / Researchers** | Sections 4–6 | Causal Foundations · RDD · DiD · PSM · DIF · Factor Analysis · Jacobson-Truax · Norm-Score Distortion |

---

## 🛠 Built With

Vanilla JS · HTML5 Canvas · No framework · No build step · Runs entirely in the browser.

---

## 📚 Methodological Grounding

The tools build on foundational work across applied statistics, psychometrics, and causal inference, including:

| Area | Key References |
| :--- | :--- |
| **Causal inference** | Pearl (DAGs, d-separation) · Rubin (potential outcomes) · Imbens & Lehner (RDD) |
| **Clinical change** | Jacobson & Truax (1991, RCI & clinical significance) · Lienert & Raatz (area transformation) |
| **Effect sizes & power** | Cohen (1988) · Lakens (2022, sample-size justification, SESOI) |
| **Psychometrics** | Lord & Novick (test theory) · Samejima, Masters, Muraki (IRT) · Shrout & Fleiss (ICC) |
| **Paradoxes** | Galton (regression to the mean) · Berkson · Lord · Simpson |

> All external references and conceptual frameworks belong to their respective authors. This project is released under the MIT License.

---

## 🔗 Sister Project — Bayes Thinking Lab

Frequentist methods are at home here — but for priors, posterior distributions, ROPE decisions, Bayes factors, and `brms` model building there is the **[Bayes Thinking Lab](https://www.bayes-thinking-lab.uni-osnabrueck.de/)**: 21 interactive tools that teach Bayesian thinking from the ground up. The two labs complement each other — *Lindley's Paradox*, for instance, needs both perspectives.

🌐 [www.bayes-thinking-lab.uni-osnabrueck.de](https://www.bayes-thinking-lab.uni-osnabrueck.de/) · 💻 [github.com/raduesing/Bayes_Thinking_Lab](https://github.com/raduesing/Bayes_Thinking_Lab)

---

## 🎓 Citation

If you use the **Methods Lab** for research, teaching, or software development, please cite it as follows:

<div align="left">

### APA Style
> Düsing, R. (2026). *Methods Lab: An interactive suite of statistical methods tools for teaching and research.* GitHub. https://github.com/raduesing/MethodsLab

### BibTeX
```bibtex
@software{Duesing_Methods_Lab_2026,
  author  = {Düsing, Rainer},
  title   = {{Methods Lab: An interactive suite of statistical methods tools for teaching and research}},
  url     = {https://github.com/raduesing/MethodsLab},
  year    = {2026}
}
```

</div>

---

## 📬 Contact

**Methods Lab** · University of Osnabrück
Fachgebiet Forschungsmethodik, Diagnostik & Evaluation
Dr. Rainer Düsing · [ResearchGate](https://www.researchgate.net/profile/Rainer-Duesing)
✉️ [methods-lab@uni-osnabrueck.de](mailto:methods-lab@uni-osnabrueck.de)

---

<div align="center">
<sub>Built for teaching. Runs in any browser. No data ever leaves your machine.</sub>
</div>
