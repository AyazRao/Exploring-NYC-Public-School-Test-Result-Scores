# Exploring-NYC-Public-School-Test-Result-Scores
Use data manipulation and summary statistics to analyze test scores across New York City's public schools!

# NYC Public School SAT Performance Analysis

## Project Overview

Every year, American high school students take SATs, standardized tests measuring literacy, numeracy, and writing skills. With three sections - reading, math, and writing - each with a maximum score of 800 points, SATs are crucial for students and colleges, playing a pivotal role in the admissions process.

Analyzing school performance is essential for various stakeholders, including policy and education professionals, researchers, government officials, and parents making decisions about their children's education.

This project focuses on analyzing SAT scores in New York City schools with the aim of identifying schools with the best math scores, determining the top 10 performing schools, and locating the NYC borough with the largest standard deviation in SAT performance.

## Dataset Preview

The dataset `schools.csv` provides information about schools in NYC, including SAT scores. A preview of the dataset is as follows:

```plaintext
| school_name   | borough   | building_code | average_math | average_reading | average_writing | percent_tested  |
|---------------|---------  |---------------|--------------|-----------------|-----------------|-----------------|
| School A      | Manhattan | M022          | 750          | 780             | 760             | 90%             |
| School B      | Brooklyn  | M445          | 800          | 790             | 780             | 95%             |
| ...           | ...       | ...           | ...          | ...             | ...             | ...             |
```

## Getting Started

To run the analysis locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/AyazRao/Exploring-NYC-Public-School-Test-Result-Scores.git
   cd sat-scores-analysis
   
## Project Structure

- `dataset/`: Contains the dataset used for analysis and modeling.
- `notebooks/`: Jupyter notebooks for exploratory data analysis, feature engineering, and modeling.
- `images/`: Visualizations and plots generated during the analysis.

## Objectives

### 1. Finding schools with the best math scores

- **Objective:** Subset the data to identify schools with math scores of at least 80%.

### 2. Identifying the top 10 performing schools

- **Objective:** Create a column named "total_SAT" by summing the scores across the three SAT sections, sort the data, and extract the top 10 schools.

### 3. Locating the NYC borough with the largest standard deviation

- **Objective:** Group the data by borough, calculate statistics, and identify the borough with the largest standard deviation in SAT performance.

## How to Approach the Project

### 1. Finding schools with the best math scores

- **Instructions:**
  1. Subset the data to find schools with math scores of at least 80%.

### 2. Identifying the top 10 performing schools

- **Instructions:**
  1. Add a new column named "total_SAT" to the original DataFrame.
  2. Sort the DataFrame by "total_SAT" in descending order.
  3. Subset the DataFrame for the "school_name" and "total_SAT" columns to get the top 10 schools.

### 3. Locating the NYC borough with the largest standard deviation

- **Instructions:**
  1. Group the data by "borough" and calculate the number of schools, mean, and standard deviation of "total_SAT."
  2. Identify the borough with the largest standard deviation.
  3. Rename columns for clarity.
