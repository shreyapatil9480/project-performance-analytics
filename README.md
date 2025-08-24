# Project Performance Analysis

This repository contains a synthetic dataset and an analysis notebook designed to showcase skills relevant for **business analyst**, **program manager**, and **data analyst** roles. The project explores factors affecting project delays and completion times and builds predictive models to classify whether a project will experience a delay.

## Dataset

The `project_performance_dataset.csv` file contains 200 rows of synthetic project data. Each row represents a project task with the following columns:

- `ProjectID` – unique identifier for the project.
- `StartDate` – start date of the task.
- `EndDate` – end date (start date + duration + delay).
- `BaseDurationDays` – planned duration in days.
- `TeamSize` – number of people assigned to the task.
- `Budget` – project budget in USD.
- `ComplexityScore` – score from 1 (low) to 10 (high) representing task complexity.
- `RiskScore` – score from 1 (low) to 10 (high) representing project risk.
- `DelayFlag` – binary flag indicating whether the project experienced a delay (`1`) or not (`0`).
- `DelayDays` – number of days delayed (0 if no delay).
- `CompletionTimeDays` – actual completion time (planned duration + delay).
- `StakeholderEngagement` – score from 1 to 10 indicating stakeholder involvement.
- `Domain` – categorical variable describing the business domain (IT, Marketing, Finance, HR, Operations).

## Analysis Notebook

The Jupyter notebook `project_analysis.ipynb` performs an exploratory data analysis (EDA) and builds predictive models to classify project delays. The notebook includes:

- Loading and exploring the dataset
- Visualising distributions, scatter plots, bar charts, and a correlation heatmap
- Splitting the data into training and testing sets
- Training a logistic regression and a random forest classifier
- Evaluating model performance and interpreting feature importance
- Summarising the findings

The notebook is fully executable; all necessary Python libraries are listed in `requirements.txt`.

## Getting Started

1. Clone this repository:

   ```bash
   git clone <repository-url>
   cd <repository-name>
   ```

2. Create a virtual environment (optional) and install dependencies:

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. Launch Jupyter Notebook to explore the analysis:

   ```bash
   jupyter notebook project_analysis.ipynb
   ```

The dataset file `project_performance_dataset.csv` is automatically loaded by the notebook. You can modify the notebook to perform additional analyses or extend the dataset.

## Repository Structure

- `project_performance_dataset.csv` – synthetic project performance data.
- `project_analysis.ipynb` – Jupyter notebook with EDA and predictive modeling.
- `requirements.txt` – Python package dependencies.
- `README.md` – overview and instructions.

## Contributing

This project is intended as an out-of-the-box example for practicing business and data analysis. Feel free to fork the repository, adapt the dataset or notebook for your own purposes, and submit pull requests with enhancements.

## Usage

To explore the analysis yourself, clone the repository and open the `project_analysis.ipynb` notebook in Jupyter. You can adjust the code to explore additional questions or modify the synthetic dataset to simulate new scenarios.
