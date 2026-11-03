# Reproducible gmx_MMPBSA + Entropy + Per-Residue Pipeline

**Author:** Sahar Wajahat
**Date:** November 2026
**License:** MIT — Free for academic/non-commercial use
**Contact:** saharwajahatfuuast@gmail.com
**ORCID:** [0009-0001-9005-5448](https://orcid.org/0009-0001-9005-5448)

---

### Citation
If you use this software in your research, please cite:

> Wajahat, S. (2026). *gmx_MMPBSA-Analysis-Template-GB-PB-Entropy-Decomp-Heatmap: Reproducible gmx_MMPBSA Workflow for Binding Free Energy* (Version 1.0.0) [Computer software]. https://github.com/SaharWajahat/gmx_MMPBSA-Analysis-Template-GB-PB-Entropy-Decomp-Heatmap

---

### 1. Purpose
A complete, end-to-end Colab notebook for **MM/GBSA & MM/PBSA** binding free energy analysis from GROMACS MD trajectories. Designed for reproducibility, transparency, and publication-ready plots. Focus on Protein-LIG systems.

### 2. What This Pipeline Does
1.  **Parse gmx_MMPBSA outputs:** `FINAL_DECOMP_last10ns_lig_23.csv` + `FINAL_DECOMP_last10ns_lig_23.dat` + `FINAL_RESULTS_last10ns_lig_23.csv` + `FINAL_RESULTS_last10ns_lig_23.dat` (GB/PB)
2.  **Incorporate NMODE Entropy:** Correct binding energy with -TΔS for realistic ΔG
3.  **GB vs PB Comparison:** Side-by-side energy comparison (LIG_23 - GB vs PB)
4.  **Per-Residue Decomposition:** Identify key hotspot residues driving binding
5.  **Generate Publication Plots:** Heatmaps, bar plots, energy vs time - all 300 dpi
6.  **Export all outputs:** `.png` figures for thesis/paper
