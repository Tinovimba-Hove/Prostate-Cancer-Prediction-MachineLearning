# Enhanced Prediction of Prostate Cancer Using PVT1 Biomarkers and PSA

## Introduction
Prostate cancer (PCa) is the second leading cause of cancer-related deaths among men in the United States. Current screening methods primarily utilize prostate-specific antigen (PSA), which has high sensitivity for early detection but suffers from low specificity, leading to over-diagnosis and unnecessary biopsies. This study evaluates the predictive power of Plasmacytoma variant translocation 1 (PVT1) exons 4A, 4B, and 9, which are overexpressed in prostate tissues and human serum, in conjunction with PSA to improve the specificity of prostate cancer detection.

## Objective

The main objectives of this study are:
- To assess the predictive capabilities of PVT1 exons 4A, 4B, and 9 alongside PSA in detecting prostate cancer from human serum.
- To improve the specificity of PSA screening methods to reduce unnecessary biopsies.

## Data Description
The dataset includes serum biomarker measurements from men, specifically:

PSA: Serum prostate-specific antigen levels.

PVT1 Exon 4A: Level of PVT1 exon 4A in serum.

PVT1 Exon 4B: Level of PVT1 exon 4B in serum.

PVT1 Exon 9: Level of PVT1 exon 9 in serum.

PCa Status: Binary variable indicating the presence or absence of prostate cancer.

## Methodology

The analysis involved the following steps:

- Data Visualization: Visualizations of the distribution of serum biomarker data across all subjects, including boxplots and correlation matrices.
  
- Single Logistic Regression: Each biomarker was individually assessed as a predictor variable to evaluate its significance in predicting PCa status.
  
- Multiple Logistic Regression: Various pairwise combinations of biomarkers were tested to determine the optimal model for predicting PCa status.\
  
-  Area Under the Curve (AUC): AUC was calculated to evaluate the model's ability to discriminate between positive and negative cases. A higher AUC indicates better model performance.
  
- 10-Fold Cross-Validation: This method was employed to assess the model's robustness and to prevent overfitting. By dividing the dataset into ten subsets, the model was trained on nine and tested on the remaining one, ensuring that every data point was used for both training and validation.
  
- Likelihood Ratio Test (LRT): LRT was utilized to compare the goodness-of-fit between nested models. This test helps to determine whether adding predictors (e.g., PVT1 markers) significantly improves the model's performance compared to a simpler model (e.g., PSA alone).

## Results

The analysis produced the following results:

- Distribution of Data: Visualizations indicate the variability of each biomarker across the dataset, with notable differences in levels between cancer-positive and cancer-negative subjects.

- Single Logistic Regression:
Each biomarker was assessed for significance:
PSA and PVT1 exons exhibited varying levels of statistical significance, highlighting the predictive potential of each marker.

- Multiple Logistic Regression: Combinations of biomarkers led to improved model performance metrics:
Models including both PSA and PVT1 biomarkers demonstrated enhanced predictive accuracy and specificity compared to models using PSA alone.

- Key Metrics from Logistic Regression
Model Accuracy: Reflects the overall correctness of the model in predicting PCa status.
Precision and Recall: Evaluate the model's performance in identifying true positive cases while minimizing false positives.

## Discussion
The results indicate that combining PVT1 biomarkers with PSA significantly enhances the prediction of positive prostate biopsies. While PSA remains a valuable screening tool, the addition of PVT1 markers improves specificity, potentially reducing unnecessary interventions. The analysis underscores the importance of exploring multi-biomarker approaches for better clinical decision-making in prostate cancer diagnosis.

## Recommendations
Integrate PVT1 Biomarkers: Clinical guidelines should consider the integration of PVT1 exon testing with PSA to enhance prostate cancer screening protocols.
Further Research: Future studies should explore larger cohorts and additional biomarkers to further validate these findings and refine predictive models.
Address Over-Diagnosis: Ongoing efforts are needed to minimize over-diagnosis associated with PSA screening by employing more specific testing methods.

## Conclusion
This study demonstrates that the predictive power of serum biomarkers for prostate cancer can be significantly enhanced when combining PVT1 exons with serum PSA. The findings highlight the potential for improved specificity in prostate cancer screening, which could lead to better patient outcomes and reduced healthcare costs. This study is currently ongoing. 

## Usage

To replicate the analyses or further explore the data:

Clone this repository.

Ensure the required Python libraries (e.g., pandas, statsmodels, matplotlib) are installed.

Run the provided scripts to generate visualizations and logistic regression models.


