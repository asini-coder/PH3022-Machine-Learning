# PH3022 – Machine Learning and Neural Computation

Jupyter notebook exercises using the Boston Housing dataset to study linear regression, regularization, and cross-validation.

## Contents

| Notebook | Description |
| --- | --- |
| `Boston_Housing_Linear_Regression.ipynb` | Initial Boston Housing data exploration, linear regression, and train/test evaluation. |
| `Activity_01_Regularized_Regression.ipynb` | Ridge, Lasso and Elastic Net regression; alpha/l1_ratio experiments and evaluation. |
| `Activity_02_Cross_Validation.ipynb` | Linear and Lasso regression with 3-fold cross-validation, fold MSE comparisons and plotting. |

## How to run

1. Install Python 3 and Jupyter (or use Google Colab).
2. Install the Python packages: `pip install -r requirements.txt`.
3. Open a notebook in Jupyter or upload it to Google Colab.
4. Run the cells from top to bottom. A network connection is needed for the cells that retrieve the Boston Housing dataset using OpenML or the CMU data URL.

## Dataset

The notebooks retrieve the Boston Housing dataset with scikit-learn's `fetch_openml(name="boston", version=1, as_frame=True)`; the initial notebook also contains a CMU-hosted dataset-loading example. The historical dataset has known ethical and methodological limitations and is used here as assigned coursework, not as a recommended benchmark for real-world housing decisions.

## Notes on reproducibility

- These are the original uploaded notebooks, renamed for easier navigation. Their code and saved outputs have **not** been modified, corrected, or re-executed when assembling this repository.
- Some notebooks contain exploratory or earlier alternative code cells. Review the cells and run the complete notebook before treating stored output as final.
- In Activity 02, the `make_pipeline(StandardScaler(), Lasso(...))` approach is preferable for cross-validation because scaling is fitted inside each training fold.
- Stored results may differ with package versions or dataset retrieval changes.

## Tools

Python, NumPy, pandas, Matplotlib, scikit-learn, Jupyter.
