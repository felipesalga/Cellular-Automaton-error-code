# Data and artifact dictionary

| Path | Description | Provenance |
|---|---|---|
| `data/HerbaceousVegetation_723.tif` | 13-band, 64 × 64 GeoTIFF, EPSG:32630 | Input scene used by the executed notebook |
| `notebooks/*_executed.ipynb` | Full computation and saved outputs | User-executed Google Colab notebook |
| `notebooks/*_reproducible.ipynb` | Same notebook with repository-relative GeoTIFF loading | Derived release copy |
| `results/notebook_output_tables/*.csv` | Tables embedded as HTML in notebook outputs | Lossless table extraction where HTML was present |
| `results/manifest_output_tables.csv` | Cell/table index, filename, dimensions, and caption context | Generated during packaging |
| `results/expected_exports.txt` | Names of result files written by notebook code | Static inspection of notebook source |
| `config/experiment_config.yaml` | Main CA, ML, QEC, and inference parameters | Notebook configuration and manuscript |
| `config/random_seeds.txt` | Fixed seeds used by experiment | Notebook source |
| `checksums.sha256` | SHA-256 integrity checks | Generated for release |

The response variables and metrics include F1, IoU/Jaccard, balanced accuracy, precision, recall, ROC AUC, AUC-PR, logical error rate, MAE, RMSE, correlation, SSIM, PSNR, false positives, and false-alarm rate. Conditions are nominal/ideal, physical noise without syndrome-based decoding, and rotated-surface-code protection with MWPM.
