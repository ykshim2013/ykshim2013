# Youngkyu Shim

**Pediatric Neurologist · Computational Variant Analysis**

Division of Pediatric Neurology, Department of Pediatrics
Korea University Ansan Hospital, Korea University College of Medicine · Ansan, Republic of Korea

I work at the interface of pediatric epilepsy genetics and structural bioinformatics. My current
research applies physics-based ΔΔG prediction to missense variants in neurodevelopmental disease
genes, asking whether a given variant acts through **protein destabilization** or through a
**stability-neutral functional mechanism** — a distinction that sequence-based pathogenicity
predictors do not resolve. Alongside this, I build and maintain open clinical decision-support
tools for pediatric practice.

`Python` · `FoldX` · `Rosetta` `cartesian_ddG` · `AlphaFold3` · `GROMACS` · `R` · `TypeScript`

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

### Methods & protocols

Reproducible, protein-agnostic pipelines extracted from the work above.

| Repository | Scope |
|---|---|
| [foldx-stability-protocol](https://github.com/ykshim2013/foldx-stability-protocol) | End-to-end FoldX workflow — `RepairPDB` → `BuildModel` batch ΔΔG with replicate statistics |
| [rosetta-ddg-protocol](https://github.com/ykshim2013/rosetta-ddg-protocol) | Rosetta `cartesian_ddG` workflow — constrained relax → backbone-flexible ΔΔG, validated on FBXO11 and SCN2A |

---

## Clinical reference resources

| Repository | Content | |
|---|---|---|
| [Epilepsy_Gene_DB](https://github.com/ykshim2013/Epilepsy_Gene_DB) | ClinVar P/LP variant analysis with phenotype review across *SCN2A*, *EEF1A2*, *KCNQ2*, *SYNGAP1*, *CDKL5* | [Open ↗](https://ykshim2013.github.io/Epilepsy_Gene_DB/) |
| [pediatric-mogad-review](https://github.com/ykshim2013/pediatric-mogad-review) | Evidence-based review of pediatric MOGAD clinical course, PMID-verified | [Open ↗](https://ykshim2013.github.io/pediatric-mogad-review/) |
| [ASM_choice](https://github.com/ykshim2013/ASM_choice) | Antiseizure medication selection protocol | [Open ↗](https://ykshim2013.github.io/asm-choice/) |

## Clinical decision support

Browser-based calculators intended for use by clinicians at the point of care.

| Repository | Tool | |
|---|---|---|
| [pediatric-hyperkalemia-tool](https://github.com/ykshim2013/pediatric-hyperkalemia-tool) | Hyperkalemia management, ages 0–18 | [Open ↗](https://ykshim2013.github.io/pediatric-hyperkalemia-tool/) |
| [med-calculator](https://github.com/ykshim2013/med-calculator) | Weight-based dosing, IV drip rates, drug dilution | [Open ↗](https://ykshim2013.github.io/med-calculator/) |
| [electro2026](https://github.com/ykshim2013/electro2026) | Electrolyte management suite | — |
| [m-chat-screening](https://github.com/ykshim2013/m-chat-screening) | M-CHAT-R/F autism spectrum screening | — |

## Teaching

| Repository | Material | |
|---|---|---|
| [Brain_Imaging_2601](https://github.com/ykshim2013/Brain_Imaging_2601) | Pediatric brain MRI for neurologists | [Open ↗](https://ykshim2013.github.io/Brain_Imaging_2601/) |
| [Seizure_Semiology](https://github.com/ykshim2013/Seizure_Semiology) | Pediatric seizure semiology video resources | [Open ↗](https://ykshim2013.github.io/Seizure_Semiology/) |
| [PED_Neuro_seizure](https://github.com/ykshim2013/PED_Neuro_seizure) | Pediatric neurology lectures for medical students | [Open ↗](https://ykshim2013.github.io/PED_Neuro_seizure/) |

---

## Publications

<details>
<summary><strong>Peer-reviewed publications</strong></summary>

<br>

**First author**

1. **Shim Y**, Kang E, Kwak N, Kim S. Computational protein stability analysis of SCN1A missense variants reveals domain-dependent stability patterns. *Epilepsia Open*. 2026. [10.1002/epi4.70312](https://doi.org/10.1002/epi4.70312)
2. **Shim Y**, Kang E, Kim S. Computational stability analysis suggests binding-independent destabilization in pathogenic FBXO11 variants. *Scientific Reports*. 2026. [10.1038/s41598-026-57705-w](https://doi.org/10.1038/s41598-026-57705-w)
3. **Shim Y**, Lee J, Cho H, Choi EK, Shin SH, Yang DH, Jang H, Byeon JH. Recent neurodevelopmental outcomes of extremely and very preterm infants: a multicenter retrospective cohort study. *Early Human Development*. 2026. [10.1016/j.earlhumdev.2026.106606](https://doi.org/10.1016/j.earlhumdev.2026.106606)
4. **Shim Y**, Yang DH, Byeon JH, Eun BL. Adjunctive cannabidiol in intractable pediatric epilepsy: a retrospective study on tolerability, efficacy, and safety across genetic and nongenetic etiologies. *Medicine*. 2026. [10.1097/MD.0000000000047425](https://doi.org/10.1097/MD.0000000000047425)
5. **Shim Y**, Kim WJ, Kim H, Cho J, Chae JH, Kim KJ, Lim BC. Switching from oxcarbazepine to eslicarbazepine in pediatric patients with focal epilepsy is safe and well-tolerated. *Epilepsy & Behavior*. 2025. [10.1016/j.yebeh.2025.110568](https://doi.org/10.1016/j.yebeh.2025.110568)
6. **Shim Y**, Kim H, Chae JH, Kim KJ, Lim BC. Analysis of initial seizure characteristics in patients with infantile onset genetic epilepsy. *Brain & Development*. 2025. [10.1016/j.braindev.2024.104319](https://doi.org/10.1016/j.braindev.2024.104319)
7. **Shim Y**, Kim SY, Kim H, Hwang H, Chae JH, Choi J, et al. Clinical outcomes of pediatric anti-NMDA receptor encephalitis. *European Journal of Paediatric Neurology*. 2020. [10.1016/j.ejpn.2020.10.001](https://doi.org/10.1016/j.ejpn.2020.10.001)

**Co-author**

8. Woo H, **Shim Y**, Chae JH, Kim KJ, Lim BC. Seizure evolution and outcome in pediatric autoimmune encephalitis. *Pediatric Neurology*. 2023. [10.1016/j.pediatrneurol.2022.11.008](https://doi.org/10.1016/j.pediatrneurol.2022.11.008)
9. Kim SY, Lee S, Woo H, Han J, Ko YJ, **Shim Y**, et al. The Korean undiagnosed diseases program phase I: expansion of the nationwide network and the development of long-term infrastructure. *Orphanet Journal of Rare Diseases*. 2022. [10.1186/s13023-022-02520-5](https://doi.org/10.1186/s13023-022-02520-5)
10. Kim SY, **Shim Y**, Ko YJ, Park S, Jang SS, Lim BC, Kim KJ, Chae JH. Spectrum of movement disorders in GNAO1 encephalopathy: in-depth phenotyping and case-by-case analysis. *Orphanet Journal of Rare Diseases*. 2020. [10.1186/s13023-020-01594-3](https://doi.org/10.1186/s13023-020-01594-3)
11. Yoo IH, Kim W, **Shim Y**, Choi SA, Kim SY, Kim H, et al. Clinical spectrum of myelin oligodendrocyte glycoprotein-immunoglobulin G-associated disease in Korean children. *Journal of Clinical Neurology*. 2020. [10.3988/jcn.2020.16.3.461](https://doi.org/10.3988/jcn.2020.16.3.461)
12. Choi TY, Kim YK, **Shim Y**, Shin M. A stepwise household transmission of vaccine-strain varicella-zoster virus resulting in neonatal varicella. *Infection & Chemotherapy*. 2026. [10.3947/ic.2025.0133](https://doi.org/10.3947/ic.2025.0133)

</details>

---

## Contact

Open to collaboration on variant-effect prediction, epilepsy genetics, and clinical decision-support
tooling.

📧 [ykshim2013@gmail.com](mailto:ykshim2013@gmail.com)

> Clinical tools in this profile are decision-support aids for qualified healthcare professionals.
> They do not replace clinical judgment and are not a substitute for institutional protocols.
