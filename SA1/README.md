Study Overview

Study Title

Multivariate Analysis of the Physicochemical Characteristics of Red and White Wines

Research Questions

This study addresses the following research questions:

Do red and white wines differ significantly in their combined physicochemical characteristics?

Can the eleven physicochemical variables be summarized into a smaller number of principal components while retaining a substantial proportion of the total variance?

Can a smaller number of underlying factors explain the correlation patterns among the eleven physicochemical variables?

Dataset Description

The study uses the Wine Quality Dataset, which contains 6,497 wine samples, including 1,599 red wine samples and 4,898 white wine samples. Each sample includes eleven physicochemical measurements: fixed acidity, volatile acidity, citric acid, residual sugar, chlorides, free sulfur dioxide, total sulfur dioxide, density, pH, sulphates, and alcohol. The dataset also includes a quality score and a wine color label.

The combined dataset was used to compare red and white wines and investigate patterns of variation and correlation among the chemical measurements.

Dataset Source

The dataset was obtained from the UCI Machine Learning Repository.

Cortez, P., Cerdeira, A., Almeida, F., Matos, T., & Reis, J. (2009). Modeling wine preferences by data mining from physicochemical properties. Decision Support Systems, 47(4), 547-553. https://doi.org/10.1016/j.dss.2009.05.016

UCI Machine Learning Repository. (2009). Wine Quality [Dataset]. https://doi.org/10.24432/C56S3T

Statistical Methods

Four main analytical approaches were used:

Exploratory Data Analysis (EDA): Descriptive statistics, distributions, boxplots, and correlation analysis were used to examine the data and identify potential outliers and relationships among variables.

Multivariate Analysis of Variance (MANOVA): Pillai's trace was used to test whether red and white wines differed in their combined mean values for five selected physicochemical variables. Follow-up ANOVAs and partial eta-squared effect sizes were used to examine individual differences.

Principal Component Analysis (PCA): The eleven physicochemical variables were standardized and analyzed to identify a smaller number of components that retained a substantial proportion of the total variance.

Exploratory Factor Analysis (EFA): KMO, Bartlett's test, parallel analysis, factor loadings, communalities, uniqueness values, and model-fit statistics were examined to explore potential underlying factors.

Summary of Major Findings

MANOVA indicated a statistically significant difference between red and white wines across the five selected physicochemical variables, with Pillai's trace = 0.78529, approximate F(5, 5314) = 3887.2, p < .001. All five follow-up ANOVAs were statistically significant after Holm adjustment, although their effect sizes varied.

PCA suggested retaining three principal components. Together, these components explained approximately 64.10% of the total variance. The components reflected patterns associated with sulfur dioxide and chemical composition, density and alcohol, and acidity-related measurements.

EFA did not produce a reliable factor solution. The overall KMO measure was 0.40, and the attempted three-factor and four-factor solutions produced inadmissible estimates for density. The three-factor model also showed poor fit. Consequently, the EFA findings were interpreted cautiously.

Overall, the analyses identified differences between red and white wines and demonstrated that PCA could summarize a substantial proportion of the variation in the physicochemical measurements. However, the EFA diagnostics limited conclusions about the underlying factor structure.

Software Used

The analyses were conducted using R in the RStudio environment. R was used for data preparation, descriptive statistics, visualization, MANOVA, follow-up ANOVAs, PCA, and EFA. The specific packages and functions used are documented in the accompanying R code.

Instructions for Reproducing the Analysis

Install R and RStudio.

Download the Wine Quality Dataset from the UCI Machine Learning Repository and place the required data files in the directory specified by the R code.

Install any required R packages that are not already available.

Open the accompanying R script or R Markdown file in RStudio.

Check that the file paths and package dependencies are correct.

Run the code from beginning to end in the order provided. The script combines the datasets, prepares the variables, conducts EDA, and performs MANOVA, PCA, and EFA.

If using R Markdown, click Knit to reproduce the report, including the written explanations, numerical output, and figures.

Compare the reproduced results with the reported findings and confirm that the analysis completes without errors.

Reproduction requires access to the original dataset, the necessary R packages, and the complete analysis code. Results may differ if the dataset, preprocessing steps, or package versions differ.
