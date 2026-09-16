# YK Shim

**Pediatric Neurologist · Computational Variant Analysis**

`Python` · `FoldX` · `Rosetta` `cartesian_ddG` · `AlphaFold3` · `GROMACS` · `R`

---

## Research

Two published studies, each with its methodology and analysis code released as a companion repository.

| Study | Approach | Repository | Publication |
|---|---|---|---|
| **SCN1A** — domain-dependent stability patterns | FoldX 5.1 + Rosetta `ref2015_cart` ΔΔG on an AlphaFold3 Nav1.1 model; ClinVar / gnomAD v4.1 stratification; benchmarked against AlphaMissense and EVE | [SCN1A-stability-analysis](https://github.com/ykshim2013/SCN1A-stability-analysis) | *Epilepsia Open* (2026) · [10.1002/epi4.70312](https://doi.org/10.1002/epi4.70312) |
| **FBXO11** — binding-independent destabilization | 44 variants × 3 AlphaFold3 seeds × 2 contexts (monomer, FBXO11–SKP1); FoldX + Rosetta + 300 ns GROMACS MD | [FBXO11_computational_framework](https://github.com/ykshim2013/FBXO11_computational_framework) | *Scientific Reports* (2026) · [10.1038/s41598-026-57705-w](https://doi.org/10.1038/s41598-026-57705-w) |

**Selected findings (SCN1A).** Predicted destabilization was associated with pathogenicity
(FoldX ROC-AUC ≈ 0.76; Rosetta concordant at Spearman ρ = 0.66). P-loop / selectivity-filter
pathogenic variants were depleted of stability-neutral cases (0.40-fold, adjusted *p* = 4.3 × 10⁻⁷),
while S4 voltage-sensor variants were enriched for them (2.32-fold, adjusted *p* = 0.013).
ΔΔG > 2.0 kcal/mol reached ≈ 0.98 specificity as supporting evidence for pathogenicity.

---

## Methods & protocols

Reproducible, protein-agnostic pipelines extracted from the work above.

| Repository | Scope |
|---|---|
| [foldx-stability-protocol](https://github.com/ykshim2013/foldx-stability-protocol) | End-to-end FoldX workflow — `RepairPDB` → `BuildModel` batch ΔΔG with replicate statistics |
| [rosetta-ddg-protocol](https://github.com/ykshim2013/rosetta-ddg-protocol) | Rosetta `cartesian_ddG` workflow — constrained relax → backbone-flexible ΔΔG, validated on FBXO11 and SCN2A |

---

## Publications

First-author articles in SCIE-indexed journals, most recent first.

1. **Shim Y**, Kang E, Kwak N, Kim S. Computational protein stability analysis of *SCN1A* missense variants reveals domain-dependent stability patterns. *Epilepsia Open*. 2026. [10.1002/epi4.70312](https://doi.org/10.1002/epi4.70312)
2. **Shim Y**, Kang E, Kim S. Computational stability analysis suggests binding-independent destabilization in pathogenic *FBXO11* variants. *Scientific Reports*. 2026;16(1):27743. [10.1038/s41598-026-57705-w](https://doi.org/10.1038/s41598-026-57705-w)
3. **Shim Y**, Lee J, Cho H, Choi EK, Shin SH, Yang DH, Jang H, Byeon JH. Recent neurodevelopmental outcomes of extremely and very preterm infants: a multicenter retrospective cohort study. *Early Human Development*. 2026;221:106606. [10.1016/j.earlhumdev.2026.106606](https://doi.org/10.1016/j.earlhumdev.2026.106606)
4. **Shim YK**, Lee YH, Choe YJ, Yoon Y, Kim YK. Cohort profile: Korean Varicella Immunization Monitoring (K-VIM) Scheme — a national cohort of children born 2011–2022. *Epidemiology and Health*. 2026;48:e2026005. [10.4178/epih.e2026005](https://doi.org/10.4178/epih.e2026005)
5. **Shim Y**, Yang DH, Byeon JH, Eun BL. Adjunctive cannabidiol in intractable pediatric epilepsy: a retrospective study on tolerability, efficacy, and safety across genetic and nongenetic etiologies. *Medicine*. 2026;105(5):e47425. [10.1097/MD.0000000000047425](https://doi.org/10.1097/MD.0000000000047425)
6. **Shim Y**, Kim WJ, Kim H, Cho J, Chae JH, Kim KJ, Lim BC. Switching from oxcarbazepine to eslicarbazepine in pediatric patients with focal epilepsy is safe and well-tolerated. *Epilepsy & Behavior*. 2025;173:110568. [10.1016/j.yebeh.2025.110568](https://doi.org/10.1016/j.yebeh.2025.110568)
7. **Shim Y**, Kim H, Chae JH, Kim KJ, Lim BC. Analysis of initial seizure characteristics in patients with infantile onset genetic epilepsy. *Brain & Development*. 2025;47(1):104319. [10.1016/j.braindev.2024.104319](https://doi.org/10.1016/j.braindev.2024.104319)
8. **Shim Y**, Kim SY, Kim H, Hwang H, Chae JH, Choi J, et al. Clinical outcomes of pediatric anti-NMDA receptor encephalitis. *European Journal of Paediatric Neurology*. 2020;29:87–91. [10.1016/j.ejpn.2020.10.001](https://doi.org/10.1016/j.ejpn.2020.10.001)

---

## Contact

Open to collaboration on variant-effect prediction and epilepsy genetics.

📧 [ykshim2013@gmail.com](mailto:ykshim2013@gmail.com)
