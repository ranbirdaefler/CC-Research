Analysis-PerDatasetModel.ipynb
A notebook for exploratory analysis of the MCF7 and HCC1806 SmartSeq datasets, followed by the development of two cell-line-specific predictive models. Each model is trained and optimized separately for its own dataset, so the hyperparameters are tuned specifically for MCF7 and HCC1806 predictions, respectively.

Combined_CellLine_Model.ipynb
A notebook that investigates cross-cell-line hypoxia vs. normoxia prediction. It includes a combined pooled model trained on both MCF7 and HCC1806, as well as a binning-based approach designed to improve generalization to unseen datasets. The notebook compares cross-dataset transfer performance against the cell-line-specific baselines.

Figures/
A folder containing visual summaries of model performance:

binning...png: performance results for the binning-based model
combinedmodel...png: performance results for the combined pooled model without binning
MCF7 and HCC: plots for the cell-line-specific models, including cross-validation results and held-out test set performance for models trained and evaluated on their respective datasets
