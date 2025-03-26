# NMIBC Risk Stratification using Cox Proportional Hazards Modeling

This repository implements a survival analysis pipeline for predicting recurrence-free survival in non-muscle-invasive bladder cancer (NMIBC) patients using clinical data and gene expression profiles. The model is based on a regularized Cox Proportional Hazards model trained on the UROMOL teaching cohort and externally validated on the Knowles dataset.

## File Descriptions

- **`UROMOL_TaLG_teachingcohort.csv`**  
  Clinical and gene expression data for the training cohort (UROMOL). The original R `.rds` file was converted to CSV format using R and uploaded here for Python compatibility.

- **`knowles_matched_TaLG_final.csv`**  
  External validation cohort with aligned clinical and expression data.

- **`model.ipynb`**  
  Jupyter notebook containing the full data preprocessing, PCA transformation, model training, internal/external validation, risk stratification, and visualization steps.

- **`requirements.txt`**  
  Contains all required Python packages and versions used in the analysis.

---

## How to Run

1. **Install Dependencies**

   Create a virtual environment and install the required packages:

   ```bash
   pip install -r requirements.txt
