# T9 – SVM Classification on the Forest Cover Type Dataset

This project uses the real-world Forest Cover Type dataset to classify forest cover into seven classes using Support Vector Machines (SVM).

## Methods included

- Dataset inspection and cleaning
- Missing-value handling with `SimpleImputer`
- Feature standardization with `StandardScaler`
- Stratified train/test split
- Linear SVM
- Polynomial SVM
- RBF SVM
- Accuracy and classification-report evaluation
- PCA-based 2D decision-boundary visualizations for each kernel

## Dataset

The notebook expects the UCI/Covertype data file named `covtype.data` in the same folder as the notebook.

The dataset has no header row. The notebook assigns column names to its 54 input features and target (`Cover_Type`).

Download the Forest Cover Type dataset from a trusted dataset source, then place `covtype.data` beside the notebook. The dataset file is intentionally not included in this repository because it is large.

## Run the project

1. Install Python and Jupyter Notebook (or use Anaconda).
2. Download `covtype.data` and place it beside `T9_SVM_Forest_Cover.ipynb`.
3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Open the notebook and run the cells from top to bottom.

The notebook samples up to 5,000 rows to make SVM training more manageable on a typical computer.

## Notes

- The three main models are trained on the standardized feature set.
- PCA is used for 2D visualization. The visualization-specific SVM models are separate from the full-feature models, so their plots are not the same models used for the reported full-feature accuracy.
- Results may vary slightly with library versions and dataset contents.
