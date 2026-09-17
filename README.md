# geometry_working_memory

Code of manuscript: Santo-Angles A, Gyurkovics M, Jaworska K, Palva JM, Thut G, Palva S. Working memory operations emerge from dynamic changes in neural subspace geometry. bioRxiv. 2026. Preprint. doi: 10.64898/2026.08.31.748237

To facilitate reproducibility, data is available at the OSF repository. We provide the neural activity matrices (X) used to compute the neural subspaces. 

To run the analyses, download the GitHub repository and place it in path_to_local/scripts, and download the OSF repository and place it in path_to_local/results.

The expected runtime of the entire pipeline is approximately 12 hours, depending on the computational environment and configuration.

## software

The code was developed and tested using Python 3.13.0 on a Mac laptop and Python 3.9.25 on the CSC Puhti and Roihu high-performance computing (HPC) clusters. The software is made publicly available under the MIT License.

## scripts

- script_01_pca.ipynb

Compute subspaces (PC scores).

- script_02_hyperalignment_pc_scores.ipynb

Hyperalignment of PC scores across subjects.

- script_03_separability_metrics.ipynb

Compute separability metrics (euclidean distance).

- script_04_alignment_metrics.ipynb

Compute alignment metrics (Principal Angle and Variance Accounted For).

- script_05_procrustes_shape_metrics.ipynb

Compute shape metrics (procrusted distance).

- script_06_surrogate.ipynb

Compute surrogate data. Set variable ‘number_permutations’ to 1000 to reproduce the procedure used in the paper. It is currently set to 5 for debugging purposes.

- script_07_stats_figures_separability.ipynb

Stats and figures on separability metrics. 

- script_08_stats_figures_alignment.ipynb

Stats and figures on alignment metrics (PA and VAF).

- script_09_stats_figures_procrustes.ipynb

Stats and figures on shape metrics (procrustes distance).

