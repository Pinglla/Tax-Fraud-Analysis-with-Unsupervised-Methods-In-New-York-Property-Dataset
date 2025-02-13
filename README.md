# Tax-Fraud-Analysis-with-Unsupervised-Methods-In-New-York-Property-Dataset

## Project Overview

### Introduction
Tax fraud poses a significant challenge to public revenue and economic stability. As technological advancements provide more avenues for tax evasion, developing robust fraud detection systems is crucial. This project leverages unsupervised machine learning methods to identify potential tax fraud within the New York property dataset, helping authorities focus their investigative efforts on high-risk cases.

### Objective
The goal of this project is to detect anomalies in property tax records by using unsupervised learning techniques. By identifying patterns in property valuation, land usage, and tax classifications, we aim to highlight records that may be indicative of tax fraud.

### Methodology
1. Data Acquisition & Preprocessing
   - The dataset consists of 1,070,994 property records from New York, covering 32 fields with a mix of numerical and categorical variables (14 numeric, 18 categorical).
   - Data cleaning involved handling missing values, correcting inconsistencies, and filtering out non-relevant records (e.g., government-owned properties).

2. Feature Engineering & Selection
   - Additional variables were created to analyze property size, valuation, and classification.
   - Key features include price per square foot, land-to-building ratios, and deviations from tax-class averages.
   - Dimensionality reduction was performed using Principal Component Analysis (PCA) to address high dimensionality and correlation among features.

3. Anomaly Detection Algorithms
   - Two unsupervised learning methods were applied to detect tax fraud:
     a. Z-Score Outlier Detection: Measures the distance of records from the mean using Minkowski distance.
     b. Autoencoder-Based Anomaly Detection: A deep learning model trained to reconstruct data, where high reconstruction errors indicate potential fraud.
   - Final fraud scores were computed by averaging the ranking of both methods.

4. Validation & Case Study
   - High-scoring records were manually reviewed using external sources such as Google Maps.
   - Three key cases were identified with substantial inconsistencies in property valuation and classification, warranting further investigation by tax authorities.

### Key Findings
- Properties with abnormally low assessed values relative to their market value were strong indicators of potential tax fraud.
- Anomalies in lot dimensions, building structures, and tax class assignments suggested possible underreporting.
- A review of top-ranked records identified several cases that warrant further expert investigation.

### Conclusion & Future Work
This project successfully applied unsupervised learning techniques to detect tax fraud in property records. Future improvements include:
- Collaboration with tax professionals to refine fraud indicators and validate findings.
- Integration with real-time tax assessment systems for proactive fraud prevention.
- Expanding the model to other municipalities to improve fraud detection strategies at a broader scale.

By leveraging machine learning, municipalities can enhance tax compliance enforcement, reduce revenue losses, and maintain fairness in property taxation.


P.S The foundational code for this project was provided by the professor, and my primary task involved refining the code and adapting it to achieve the desired outputs.

