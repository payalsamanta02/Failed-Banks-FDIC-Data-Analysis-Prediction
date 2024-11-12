# Failed-Banks-FDIC-Data-Analysis-Prediction
Failed US Banks FDIC Data Analysis and Prediction


This repository contains code for an Exploratory Data Analysis (EDA) of failed bank data from the FDIC.

**Project Description: Predicting U.S. Bank Failures Using FDIC Financial Ratios**  

In this project, I developed a predictive model to identify potential bank failures within 180 days using historical financial ratios from the FDIC database. The dataset included 796 features and 656,438 training examples spanning the past 90 quarters. The binary target label classified banks as likely to fail or not, with a positive instance indicating failure within 180 days.  

The 180-day prediction window was chosen to account for the FDIC's data reporting lag of 60–90 days and optimize model performance. Precision was prioritized over recall to minimize false positives, crucial for high-stakes decision-making in banking.  

Key highlights include:  
- **Model Development:** Applied machine learning techniques to train and evaluate models, with hyperparameters tuned using HyperOpt for optimal performance.  
- **Performance Metrics:** The best model achieved an AUC of 0.636, an F1 score of 0.413, and a precision of 0.83 on the test set, demonstrating its reliability in identifying high-risk banks.  
- **Feature Engineering:** Leveraged 796 financial ratios and historical data to identify patterns indicative of bank instability.  

This project provides valuable insights into financial risk assessment, supporting regulatory bodies and stakeholders in proactive decision-making.

### Getting Started

1.  **Prerequisites:**

<!-- end list -->

  - R software: [[https://www.r-project.org/](https://www.google.com/url?sa=E&source=gmail&q=https://www.r-project.org/)]
  - Required R packages:
      - tidyverse
      - ggplot2
      - dplyr
      - moments
      - viridisLite
      - viridis

<!-- end list -->

2.  **Download and Set Up:**

<!-- end list -->

  - Clone this repository to your local machine.
  - Open R and navigate to the directory containing the R script (`Failed_Bank_Dataset_2.csv` and this README file).
  - Install the required R packages if you haven't already:
    ```r
    install.packages("tidyverse")
    install.packages("ggplot2")
    install.packages("dplyr")
    install.packages("moments")
    install.packages("viridisLite")
    install.packages("viridis")
    ```

<!-- end list -->

3.  **Run the Script:**

<!-- end list -->

```r
library(tidyverse)
library(ggplot2)
library(dplyr)
library(moments)
library(viridisLite)
library(viridis)
# ... rest of the script code
```

### Content of the Repository

  - `Failed_Bank_Dataset_2.csv`: The failed bank data used for the analysis.
  - `Failed_Banks_EDA.R`: The R script containing the code for the EDA.
  - `README.md`: This file (you are reading it now\!).

### Description of the Script

The script performs the following steps:

1.  **Imports:** Imports libraries and the dataset.
2.  **Questions to Explore:** Defines questions to be addressed by the analysis.
3.  **Data Cleaning:** Checks data structure and quality, removes missing values, and adds a 'Year' column.
4.  **Data Transformation:** Explores distributions with square root and log transformations.
5.  **Bank Failures & Losses Per Year:** Analyzes the number of failed banks and estimated losses per year since 2000.
6.  **Bank Failures & Losses By State:** Explores  bank failures and estimated losses by state.
7.  **Ratio Analysis:** Analyzes the deposits to assets ratio and the estimated loss to assets ratio, and investigates the relationship between them.

The script generates various visualizations to explore different aspects of the data.

### License

This code is provided under the MIT License. See the LICENSE file for more details.
