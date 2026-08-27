<div align="center">

# Methods Lab `beta 0.7`
### Statistical Methods, Made Tangible.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Static Badge](https://img.shields.io/badge/Status-Academic_Project-blue)]()
[![Static Badge](https://img.shields.io/badge/Tech-Vanilla_JS-orange)]()
[![Static Badge](https://img.shields.io/badge/Tools-46_interactive-green)]()
[![Static Badge](https://img.shields.io/badge/Version-0.7_beta-lightgrey)]()

### 🌐 [www.methodslab.uni-osnabrueck.de](https://www.methodslab.uni-osnabrueck.de/)

**A suite of 46 interactive tools that build statistical intuition from the ground up — from OLS regression, ANOVA and multilevel models, through the counter-intuitive paradoxes that trip up even seasoned researchers, into modern causal inference, psychometrics (classical test theory, measurement models, reliability, IRT), and clinical diagnostics. Everything runs entirely in the browser. No code, no server, no data ever leaves your machine.**

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
| **1 · Regression & Relationships** | How linear relationships are estimated and decomposed — the foundation for everything else | OLS Regression · Partial Correlation · Mediation · Moderation · ANOVA · Multilevel Models |
| **2 · Inference & Planning** | What a p-value actually claims, how big a sample needs to be, what counts as a meaningful effect, and what missing data does | Significance Tests · Effect Sizes · Power & Sample Size · Missing Data |
| **3 · Statistical Paradoxes** | Why counter-intuitive results are, in fact, plain regression or sampling logic | Regression to the Mean · Attenuation · Berkson · Lord · Simpson · Law of Small Numbers |
| **4 · Causal Inference** | When association may be read as causation — and the toolkit of modern causal analysis | Causal Foundations · RDD · Difference-in-Differences · Propensity Score Matching |
| **5 · Test Theory & Measurement** | How psychological constructs are measured and how well | Classical Test Theory · Measurement Models (CFA) · Factor Analysis · Reliability (α vs. ω) · IRT · DIF |
| **6 · Diagnostics & Test Quality** | How accurately an instrument detects what it should — at the level of the individual | Sensitivity/Specificity · Diagnostic Validity · Taylor-Russell · ICC · Diagnostic Intervals · Norm-Score Distortion · Jacobson-Truax |

---

## 🛠 The Ecosystem

Legend: **✓** finished · **◷** planned

### 1 · Regression & Relationships
*The foundation: how to estimate linear relationships, what "controlling for" means, and how effects split into direct and indirect paths.*

* **✓ OLS & Multiple Regression** — Simple and multiple regression: coefficients, R², assumptions, and typical violations. Interactive data injection.
* **✓ Partial Correlation** — The correlation of two variables purged of a third. Suppressor effects, semi-partial correlation, path coefficients.
* **✓ Mediation Analysis** — Hayes/PROCESS Model 4: DAG visualization, direct and indirect effect, Sobel/Aroian live, bootstrap on demand.
* **✓ Moderation Analysis** — Hayes/PROCESS Model 1: simple slopes, Johnson-Neyman technique, floodlight plot. When does W moderate the effect of X on Y?
* **✓ ANOVA** — One-way and two-way analysis of variance with interaction — the same dataset recomputed as a regression with dummy vs. effect coding. Same F, same p, different parametrization.
* **✓ Multilevel Models** — Complete / no / partial pooling compared, shrinkage caterpillar plot, ICC slider, random slopes (τ₁, ρ), Simpson's paradox experienced live, plus a dedicated "Shrinkage Extreme" module showing when and why partial pooling improves out-of-sample prediction for small/unbalanced groups.

### 2 · Inference & Planning
*How large must a sample be? What is a meaningful effect? And what happens when data are missing?*

* **✓ Significance Tests** — What a p-value actually claims: repeated draws under H₀ make the definition tangible, the "dance of the p-values" shows its instability. Five classic misinterpretations corrected.
* **✓ Effect Sizes** — Cohen's d, r, η², f, OR/RR: conversions, visualizations, confidence intervals.
* **✓ Effect Size Calculator** — Exact computation on your own data: CSV upload, d_z/d_rm/d_av, Student's t vs. Welch's t side by side, Hedges/Nakagawa/Bonett corrections, confidence intervals via Bonett, Rosenthal, and the noncentral t-distribution.
* **✓ Power & Sample Size** — Four-curve family, H₀/H₁ distributions, n×d heatmap, sensitivity curve, MDES, SESOI. α, β, d, n fully interactive.
* **✓ Missing Data** — MCAR, MAR, MNAR: understand the mechanisms, compare four imputation strategies, traffic-light grid for bias and efficiency.

### 3 · Statistical Paradoxes
*Counter-intuitive effects that trap even experienced researchers. All of them rest on regression logic — which is why this section comes after the foundations.*

* **✓ Regression to the Mean** — Blood-pressure example, r-slider, bidirectional selection. Why "bad" extreme values look better the second time.
* **✓ Measurement-Error Attenuation** — Intelligence & school achievement: disattenuation, learning cards on N-instability and reliability choice.
* **✓ Berkson's Paradox** — Talent + effort → success: DAG, diagonal selection boundary, collider bias. Negative correlation in selected samples.
* **✓ Lord's Paradox** — ANCOVA vs. change scores: when do the two analyses lead to opposite conclusions? DAG, key formula, lege-artis decision.
* **✓ Simpson's Paradox** — An aggregate (pooled) trend reverses on disaggregation: within- vs. pooled regression, confounding slider, reversal & amplification scenarios. Cross-link to the multilevel tool.
* **✓ Range Restriction** — How selection on the predictor X attenuates the correlation (variance restriction). Scatter full vs. restricted, dispersion bars, the Thorndike r(u) relationship, Case-II correction. The slope stays, r shrinks. Cross-linked with Berkson and Taylor-Russell.
* **✓ Lindley's Paradox** — p < .05 yet the Bayes factor supports H₀: the frequentist–Bayes conflict. Lindley mode, z-distribution H₀ vs. H₁, divergence over n. Synergy with the Bayes Thinking Lab.
* **✓ Will Rogers Phenomenon** — When the Okies left Oklahoma for California, the average IQ of both states rose. Reclassification raises the mean of both groups at once, while the overall mean stays put — animated. Also: stage migration.
* **✓ Data Dredging & the Streetlight Paradox** — Search a large dataset for significance and you will find spurious hits by chance. Multiple comparisons, P(≥1)=1−(1−α)ᵐ, Bonferroni, HARKing headlines, plus stepwise regression (Freedman) — spuriously significant predictors, R² inflation.
* **✓ Inspection Paradox** — You land by chance in above-average-length intervals (buses, clinical cohorts, survival data). Length-biased sampling: the experienced gap = E[L²]/E[L] ≥ E[L].
* **✓ Survivorship Bias** — Wald's bombers: where to add armor? Mark the damaged zones, then reveal — the missing (shot-down) planes show where it actually matters. Selecting on the outcome distorts every conclusion drawn from survivors alone.
* **✓ Law of Small Numbers** — The "record" municipalities (highest and lowest rates) are systematically the smallest — pure sampling variance, not a real effect. Funnel plot, ranked list, SE ∝ 1/√n. Related to Regression to the Mean.
* **✓ Friendship Paradox** — Your friends have more friends than you do, on average — size-biased sampling over edges. Click people, make a prediction, reveal. Related to the Inspection Paradox.

### 4 · Causal Inference
*Under what conditions may association be read as causation? The potential-outcomes framework, natural experiments, and matching.*

* **✓ Causal Inference — Foundations** — DAGs, potential outcomes, IPW, G-computation: five modules in a full-screen layout. Strong confounding, live ATE estimation.
* **✓ Regression Discontinuity (RDD)** — Sharp RDD: scenarios A–D, polynomial-degree slider, fuzzy RDD, and polynomial pitfalls as expandable modules.
* **✓ Difference-in-Differences** — Regression model, ATT, selection bias, naïve comparisons, live-updating arrows. The parallel-trends assumption made visual.
* **✓ Propensity Score Matching** — Logistic PS estimation, greedy 1:1 matching, IPW (ATT), love plot, estimator comparison before/after matching.

### 5 · Test Theory & Measurement
*How psychological constructs are measured — and how well a test does that. Ordered as a learning path: classical foundations → latent measurement models → reliability → modern IRT.*

* **✓ Classical Test Theory — Basics** — True-score model X = T + E, reliability as a variance ratio, SEM, confidence band around a single test score, Spearman-Brown test-length prophecy. The anchor of the whole reliability theme.
* **✓ Measurement Models (CFA intro)** — Parallel, tau-equivalent, congeneric: path diagram, implied covariance matrix, automatic model classification, ω_total vs. α live, optional intercepts for essential equivalence. The bridge from factor analysis to reliability.
* **✓ Factor Analysis** — PAF (genuine EFA), correct oblique solution (pattern matrix Λ), reliability panel (α / ωt / ωh Schmid-Leiman), three scenarios, biplot.
* **✓ Reliability: α vs. ω** — Cronbach's α vs. McDonald's ω_total / ω_hierarchical: when α *underestimates* (congeneric) and when it *feigns unidimensionality* (multidimensional). Variance decomposition, split-half distribution, three scenarios.
* **✓ IRT — Dichotomous Models** — 1PL/2PL/3PL/4PL + Rasch: ICC, TIF, Wright map, MLE person estimation. The Rasch-vs-1PL distinction made explicit.
* **✓ IRT — Ordinal Models** — PCM, GPCM, GRM: CRF, ESC, item information for every item. Disordered-threshold warning, factor-analysis link in the help.
* **✓ Differential Item Functioning (DIF)** — 2PL model, four items, Δb/Δa sliders, ICC comparison, difference curve, group distributions, Raju SA/UA, ETS A/B/C.
* **✓ Measurement Invariance** — Configural / metric / scalar: the CFA twin of DIF. Set a true difference and a degree of non-invariance and see how much of a group difference is real vs. a measurement artifact.
* **◷ Generalizability Theory** — G-theory as the multi-facet extension of CTT: variance components across raters, items, occasions; G- and D-studies.

### 6 · Diagnostics & Test Quality
*How well does an instrument detect what it should — at the level of the individual patient?*

* **✓ Sensitivity & Specificity** — ROC curve, AUC, PPV/NPV as a function of prevalence: interactive cut-off, live 2×2 table.
* **✓ Diagnostic Validity** — Construct, criterion, and content validity: validity coefficients, Taylor-Russell tables, utility analysis.
* **✓ Taylor-Russell Tables** — The selection utility of a test: success rate (PPV) among those selected, as a function of validity, selection ratio, and base rate. Interactive table plus nomogram with a target-cross reticle; bivariate-normal computation. Cross-linked with Range Restriction.
* **✓ Test Bias** — Cleary model, Meade & Fetzer, adverse impact: three modules, four scenarios. Differential prediction vs. fairness in practice.
* **✓ Diagnostic Intervals** — Confidence, prediction, and tolerance intervals compared: what each one says and which question it answers.
* **✓ Jacobson-Truax Analysis** — Reliable Change Index & clinical significance: RCI band, cut-off criteria a/b/c/d, five-group classification (analogous to the R package JTRCI) in the pre-post plot. BDI-II and SCL-90 as worked examples.
* **✓ Norm-Score Distortion** — What linear T-scores do to right-skewed distributions (SCL-90 analogy). Gamma, log-normal, exponential, Weibull, ex-Gaussian; empirical vs. T-norm percentile ranks; area-transformation (Lienert & Raatz) overlay.
* **✓ Profile Analysis** — Profile comparison with Cattell rₚ, McCrae Iₚₐ/rₚₐ, ICC_de: elevation, scatter, and shape evaluated separately.
* **✓ ICC-Lab** — Intraclass correlation: all six Shrout-&-Fleiss forms, rater count, absolute vs. consistency agreement.
* **✓ Inter-Rater Agreement** — Cohen's κ, weighted κ, the kappa paradox, prevalence & bias: when κ misleads and what to report instead.

---

## 🚀 Getting Started

The Methods Lab is a **serverless web application**. No installation, no backend, and no data leaves your machine.

### Option 1 — Use it online (recommended)

Open the hosted version directly in your browser:

🌐 **[www.methodslab.uni-osnabrueck.de](https://www.methodslab.uni-osnabrueck.de/)**

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

## 🛠 Built With

Vanilla JS · HTML5 Canvas · No framework · No build step · Runs entirely in the browser.

---

## 🔗 Sister Project — Bayes Thinking Lab

Frequentist methods are at home here — but for priors, posterior distributions, ROPE decisions, Bayes factors, and `brms` model building there is the **[Bayes Thinking Lab](https://www.bayes-thinking-lab.uni-osnabrueck.de/)**: 21 interactive tools that teach Bayesian thinking from the ground up. The two labs complement each other — *Lindley's Paradox*, for instance, needs both perspectives.

🌐 [www.bayes-thinking-lab.uni-osnabrueck.de](https://www.bayes-thinking-lab.uni-osnabrueck.de/) · 💻 [github.com/raduesing/Bayes_Thinking_Lab](https://github.com/raduesing/Bayes_Thinking_Lab)

---

## 🎓 Citation

If you use the **Methods Lab** for research, teaching, or software development, please cite it as follows:

<div align="left">

### APA Style
> Düsing, R. (2026). *Methods Lab: An interactive suite of statistical methods tools for teaching and research* (Version 0.7 beta). GitHub. https://github.com/raduesing/MethodsLab

### BibTeX
```bibtex
@software{Duesing_Methods_Lab_2026,
  author  = {Düsing, Rainer},
  title   = {{Methods Lab: An interactive suite of statistical methods tools for teaching and research}},
  url     = {https://github.com/raduesing/MethodsLab},
  version = {0.7 beta},
  year    = {2026}
}
```

</div>

---

## 📬 Contact

**Methods Lab** · University of Osnabrück
Fachgebiet Forschungsmethodik, Diagnostik & Evaluation
Dr. Rainer Düsing · [ResearchGate](https://www.researchgate.net/profile/Rainer-Duesing)
✉️ [wwwmelab@uni-osnabrueck.de](mailto:wwwmelab@uni-osnabrueck.de)

---

<div align="center">
<sub>Built for teaching. Runs in any browser. No data ever leaves your machine.</sub>
</div>
