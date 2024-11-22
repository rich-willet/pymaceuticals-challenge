# pymaceuticals-challenge
# Define the content of the README file
readme_content = """
# Pymaceuticals Clinical Study Analysis

## Overview

This project analyzes data from a pharmaceutical study conducted by Pymaceuticals, Inc., to test the effectiveness of several drug regimens in treating squamous cell carcinoma (SCC), a form of skin cancer. Using Python and Matplotlib, we processed and visualized data to draw meaningful insights about tumor volume, treatment regimens, and their relationships with other variables like mouse weight.

## Objectives

The analysis covers the following key tasks:
1. **Prepare the Data**:
   - Merge mouse metadata and study results into a single DataFrame.
   - Identify and remove duplicate entries for accurate analysis.
2. **Generate Summary Statistics**:
   - Calculate mean, median, variance, standard deviation, and SEM for tumor volumes across each drug regimen.
3. **Create Visualizations**:
   - Generate bar plots and pie charts to visualize the data.
   - Identify trends and distributions using box plots.
4. **Explore Correlation and Regression**:
   - Examine relationships between mouse weight and tumor volume for a specific treatment regimen.
5. **Summarize Findings**:
   - Provide a top-level summary of observations based on the study's results.

## Files

- **`mouse_metadata.csv`**: Contains metadata for each mouse, including gender and drug regimen.
- **`study_results.csv`**: Contains tumor measurements over time for each mouse.
- **`pymaceuticals.ipynb`**: Jupyter Notebook containing the complete analysis and visualizations.

## Analysis Highlights

### Data Preparation
- The data includes 249 mice across various drug regimens.
- Duplicate entries based on `Mouse ID` and `Timepoint` were identified and removed.
- The cleaned dataset contained **248 unique mice**.

### Summary Statistics
For each drug regimen, the following metrics were calculated:
- **Mean Tumor Volume**
- **Median Tumor Volume**
- **Tumor Volume Variance**
- **Tumor Volume Standard Deviation**
- **Tumor Volume SEM**

### Visualizations
1. **Bar Charts**:
   - Total number of timepoints for each drug regimen.
2. **Pie Charts**:
   - Distribution of male vs. female mice in the study.
3. **Box Plot**:
   - Distribution of the final tumor volumes for the four selected drug regimens: `Capomulin`, `Ramicane`, `Infubinol`, and `Ceftamin`.

### Statistical Analysis
1. **Outlier Detection**:
   - Identified potential outliers in tumor volumes for each treatment regimen using IQR and bounds.
   - `Infubinol` had one potential outlier with a tumor volume of **36.32 mm³**.
2. **Line Plot**:
   - Visualized the tumor volume over time for a single mouse (`b742`) treated with `Capomulin`.
3. **Scatter Plot**:
   - Examined the relationship between mouse weight and tumor volume for the `Capomulin` regimen.
4. **Correlation and Regression**:
   - Correlation coefficient: **0.84**.
   - Linear regression showed a strong positive relationship between mouse weight and tumor volume.

## Key Findings
1. **Capomulin and Ramicane Are Effective**:
   - These regimens showed smaller tumor volumes on average compared to other treatments.
   - Both regimens had no potential outliers in tumor volume.
2. **Mouse Weight Correlates with Tumor Volume**:
   - Heavier mice tended to have larger tumors under the `Capomulin` regimen.
3. **Gender Distribution**:
   - The study included 51% male and 49% female mice, indicating a balanced sample.

## How to Run the Analysis

1. Clone the repository:
   ```bash
   git clone https://github.com/rich-willet/pymaceuticals-challenge.git
