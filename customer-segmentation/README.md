# Mall Customer Segmentation

Unsupervised machine learning project using KMeans clustering to identify
distinct customer segments based on annual income and spending behaviour.

## Overview

Retail businesses need to understand who their customers are in order to
run targeted marketing campaigns. This project applies KMeans clustering
to a mall customer dataset to surface five actionable customer segments —
from high-value targets to upselling opportunities.

## Dataset

- **Source:** [Kaggle — Mall Customer Segmentation Data](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)
- **Rows:** 200 customers
- **Features used:** Annual Income (k$), Spending Score (1-100)

## Methods

- Exploratory Data Analysis (distributions, scatter plots)
- Feature scaling with StandardScaler
- Optimal k selection via the Elbow Method
- KMeans clustering (k=5, random_state=42)
- Cluster profiling and business interpretation

## Key Findings

| Segment | Income | Spending | Business Action |
|---|---|---|---|
| Target customers | High | High | Loyalty programmes |
| Conservative savers | High | Low | Upselling campaigns |
| Impulsive spenders | Low | High | Discount promotions |
| Cautious spenders | Mid | Low | Targeted incentives |
| Average customers | Mid | Mid | Baseline segment |

## Project Structure
```
├── data/               # Raw dataset
├── notebooks/          # Jupyter notebook with full analysis
├── requirements.txt    # Python dependencies
└── README.md
```

## Setup
```bash
git clone https://github.com/igladko-ui/VSC-projects/mall-customer-segmentation
cd mall-customer-segmentation
pip install -r requirements.txt
jupyter notebook notebooks/segmentation.ipynb
```

## Tools & Libraries

Python 3.10+ · pandas · scikit-learn · seaborn · matplotlib