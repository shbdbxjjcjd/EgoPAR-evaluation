# EgoPAR evaluation results

These CSV files mirror the tables and the Figure 5 coordinates in the manuscript snapshot dated 2026-11-15. The experiments use the EgoChoir dataset. The manuscript refers to the original benchmark's held-out split as its validation set.

| File | Contents |
| --- | --- |
| `table1_main_results.csv` | Published comparison scores and EgoPAR's three-run mean and sample standard deviation. Scores are percentages. The geodesic error is in centimeters. Empty cells denote unavailable values. |
| `table1_b1_runs.csv` | Selected historical B1 validation rows used to calculate Table 1. `geo_m` is in meters. Other scores are on a 0–1 scale. |
| `table1_relative_improvements.csv` | Whole-percent gains relative to BSTRO for human contact and O2O for object affordance. Geodesic gains are relative error reductions. |
| `table2_component_ablation.csv` | The seven configurations reported in the manuscript. `geo_m` is in meters. Other scores are on a 0–1 scale. |
| `table3_classwise.csv` | All seven metrics for each of the 12 actions, the recorded EgoChoir reference score, and the signed difference. Columns marked `_pct` in the metric field use percentages, with differences in percentage points. `geo_cm` is in centimeters. |
| `figure5_plot_data.csv` | Ordered plot coordinates. Panel 1 uses EgoPAR minus EgoChoir AUC. Panel 2 uses EgoChoir minus EgoPAR geodesic error. |
| `table4_hyperparameter_sensitivity.csv` | The 12 sensitivity settings. Scores use the same units as Table 2. `tau_seg` and `rho_topk` are the archive names for the segmentation threshold and Top-K ratio. |
| `table3_egochoir_logged_baseline.csv` | EgoChoir's seven per-action metrics extracted from the archived evaluation log at manuscript precision. |
| `figure5_logged_evaluation.csv` | Logged per-action AUC and geodesic error for both methods, together with the 24 differences plotted in Figure 5. |
| `table2_table4_logged_checkpoints.csv` | Selected validation epochs and metrics from logged runs whose complete reported rows match Tables 2 and 4. Table 4 reports six metrics, so precision and recall are blank for its rows. |

## Class-wise evaluation

The archived per-action outputs support all EgoChoir reference scores in Table 3 and both series shown in Figure 5. The EgoChoir log does not identify the checkpoint used for the per-action evaluation.

## Citation and dataset access

For published baseline values and dataset details, cite Yang et al., *EgoChoir: Capturing 3D Human-Object Interaction Regions from Egocentric Views*, NeurIPS 2024. The source for Table 1 is Table 1 in the paper. [Paper and supplement](https://proceedings.neurips.cc/paper_files/paper/2024/hash/61f9cc83f684a4979929804ba8abf027-Abstract-Conference.html)

The authors of EgoChoir provide the dataset access instructions and terms in their project. [Official EgoChoir release](https://github.com/yyvhang/EgoChoir_release)
