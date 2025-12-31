# MR_life_course_exposures_epigenetic_aging
This repository documents a Mendelian Randomization–based causal inference pipeline to study the effects of chronic exposures on accelerated epigenetic aging, using publicly available GWAS/EWAS summary statistics under an explicit DAG-based causal framework aligned with STROBE-MR.
Research question
What is the causal effect of chronic exposure to air pollution on accelerated epigenetic aging, and to what extent is this effect mediated by systemic inflammation?
Methodological framework
The study is structured in four sequential phases:
Causal design (DAG)
Definition of the causal structure, identification of exposure, outcomes, mediators, and confounders, and validation of MR assumptions (IV1–IV3).
Instrument preparation
Selection of genetic instruments from public repositories (OpenGWAS / MR-Base), applying stringent criteria (p < 5×10⁻⁸, LD clumping, F-statistic > 10), followed by allele harmonization.
Causal inference using Mendelian Randomization
Modular MR framework, selected according to the causal question and data availability, including:
Univariable MR
Mediation MR (two-step MR)
Multivariable MR (MVMR)
Bidirectional MR
Subgroup and exploratory analyses (when applicable)
Robustness and transparency
Sensitivity analyses using IVW, MR-Egger, weighted median, heterogeneity tests, Steiger directionality test, leave-one-out analysis, and graphical diagnostics (forest, scatter, funnel plots).
Data sources
IEU OpenGWAS / MR-Base: GWAS summary statistics for environmental exposures and inflammatory biomarkers.
EWAS/GWAS consortia: Epigenetic clock outcomes derived from large-scale genomic studies.
No individual-level data are used. No new data collection was performed.
Reproducibility
All analyses are conducted in R, using established MR packages. The repository is designed to ensure transparency, reproducibility, and traceability of analytical decisions.
Ethical considerations
This study uses secondary, anonymized summary-level data from publicly available sources. Therefore, it does not require informed consent or local ethical approval.
Reporting standards
The project follows the STROBE-MR guidelines for transparent reporting of Mendelian Randomization studies.
