# gmx_MMPBSA-Analysis-Pipeline
A clean, reproducible MM/GBSA & MM/PBSA binding free energy workflow for protein-ligand analysis.

### Features
- **Parse gmx_MMPBSA outputs:** FINAL_DECOMP + FINAL_RESULTS files (GB/PB) - Tested with files from GROMACS 2023.3
- **Entropy correction:** Incorporate NMODE -TΔS for realistic ΔG
- **GB vs PB comparison:** Side-by-side energy comparison
- **Per-residue decomposition:** Identify hotspot residues
- **Analysis:** Heatmap + Bar plots + Energy vs time - all 300 dpi
- **Download:** Download results at each step to prevent data loss
- **Run on Google Colab**

[Open In Colab](https://colab.research.google.com/github/SaharWajahat/gmx_MMPBSA-Analysis-Pipeline/blob/main/gmx_MMPBSA_Analysis_Pipeline.ipynb)

### How to run:
1. Click the "Open in Colab" badge above
2. Upload your gmx_MMPBSA files: `FINAL_DECOMP_last10ns_lig_23.csv` + `FINAL_DECOMP_last10ns_lig_23.dat` + `FINAL_RESULTS_last10ns_lig_23.csv` + `FINAL_RESULTS_last10ns_lig_23.dat`
3. Run cells one by one from top to bottom
4. Edit LIG_23 variable if your ligand name is different
5. Continue running each cell to complete analysis and plots
6. Download results after each major step to prevent data loss

### Outputs
- `GB_vs_PB_comparison.png` : Side-by-side GB vs PB binding energies
- `per_residue_decomposition.png` : Hotspot residues driving binding
- `energy_heatmap.png` : Per-residue energy heatmap
- `entropy_corrected_dG.png` : Binding energy with -TΔS correction
- Status: Publication-ready figures (300 dpi)

### Citation
If you use this software, please cite:
> Wajahat, S. (2026). gmx_MMPBSA Analysis Pipeline: Reproducible Binding Free Energy Workflow with Entropy Correction, Heatmap and Per-Residue Decomposition (Version 1.0.0) [Computer software]. https://github.com/SaharWajahat/gmx_MMPBSA-Analysis-Pipeline

License: MIT

Author: Sahar Wajahat, 2026
