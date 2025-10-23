# Airbnb Pricing Analysis: Rating-Price Relationship Study

A comprehensive data science project analyzing Airbnb listings in Boston and Seattle to understand the relationship between ratings, property characteristics, and pricing strategies. This project follows the CRISP-DM (Cross-Industry Standard Process for Data Mining) methodology and is built using Python and scikit-learn.

This project was developed as part of the Udacity Data Science Nanodegree program to demonstrate end-to-end data analysis, machine learning, and stakeholder communication skills.

**Blog Post:** [Link to Medium/Blog post will be added here]

## Table of Contents

- [Overview](#overview)
- [Research Questions](#research-questions)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Methodology](#methodology)
- [Requirements](#requirements)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Overview

This project analyzes thousands of Airbnb listings from Boston (3,585 listings) and Seattle (3,818 listings) to answer critical business questions about pricing dynamics in the short-term rental market. Using machine learning techniques including Linear Regression and Random Forest models, we explore how ratings, property characteristics, and review counts influence pricing decisions.

**Dataset:** Airbnb Inside (2016 snapshot)  
**Analysis Framework:** CRISP-DM  
**Primary Tools:** Python, pandas, scikit-learn, matplotlib, seaborn

## Research Questions

This analysis addresses three main research questions:

### 1. Rating-Price Relationship by City
**Question:** In which city (Boston or Seattle) can Airbnb hosts earn more money through achieving good ratings?

### 2. Property Characteristics Impact
**Question:** Which property characteristics have the greatest impact on pricing decisions?

### 3. Review Count Optimization
**Question:** What is the optimal number of reviews for maximizing pricing potential?

## Installation

### Dependencies

This project requires:

- **Python** (>= 3.8)
- **pandas** (>= 1.5.0)
- **NumPy** (>= 1.23.0)
- **scikit-learn** (>= 1.6.0)
- **matplotlib** (>= 3.6.0)
- **seaborn** (>= 0.13.0)
- **SciPy** (>= 1.10.0)
- **openpyxl** (>= 3.1.0) - for Excel file handling

### User Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/iiPlayxX/udacity_datascience_proj_1.git
   cd udacity_datascience_proj_1
   ```

2. **Create a virtual environment (recommended):**
   ```bash
   python -m venv venv
   
   # On Windows
   venv\Scripts\activate
   
   # On macOS/Linux
   source venv/bin/activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

### Dataset Setup

The Airbnb datasets should be placed in the following structure:
```
datasets/
└── airbnb/
    ├── boston/
    │   └── versions/
    │       └── 2/
    │           └── listings.csv
    └── seattle/
        └── versions/
            └── 2/
                └── listings.csv
```

**Note:** The datasets are sourced from [Airbnb Inside](http://insideairbnb.com/get-the-data.html) and are not included in this repository due to size constraints.

## Usage

### Running the Complete Analysis

1. **Navigate to the analysis directory:**
   ```bash
   cd analysis
   ```

2. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook overview.ipynb
   ```

3. **Execute cells sequentially** to reproduce the complete analysis, or use "Run All" to execute the entire notebook.

## Project Structure

```
udacity_datascience_proj_1/
│
├── analysis/
│   └── overview.ipynb          # Main Jupyter notebook with complete analysis
│
├── datasets/
│   ├── airbnb/
│   │   ├── boston/
│   │   └── seattle/
│   └── Dataset_Summary_Airbnb.xlsx
│
├── create_dataset_summary.py   # Script to generate dataset summaries
├── question1.py                # Standalone script for Question 1 analysis
├── requirements.txt            # Project dependencies
├── README.md                   # This file
└── overview.md                 # Detailed project documentation
```

## Methodology

This project follows the **CRISP-DM** framework:

### 1. Business Understanding
- Define research questions focused on pricing optimization
- Identify stakeholders (Airbnb hosts, property managers, platform operators)
- Establish success criteria (interpretable models, actionable insights)

### 2. Data Understanding
- Exploratory Data Analysis (EDA) of 7,403 total listings
- Distribution analysis, correlation studies, and visualization
- Identification of data quality issues and patterns

### 3. Data Preparation
- Missing value handling (removed rows with missing critical features)
- Outlier removal (99th percentile threshold for price)
- Feature engineering and normalization for cross-city comparison
- Train-test split (80/20) for model validation

### 4. Modeling
- **Linear Regression:** For interpretable coefficients and relationship strength
- **Random Forest Regressor:** For feature importance and non-linear patterns
- Separate models trained for each city to capture market-specific dynamics

### 5. Evaluation
- Regression metrics: R² score (~0.50), RMSE, MAE
- Cross-city coefficient comparison with statistical interpretation
- Scenario-based predictions to validate practical utility
- Integrated visualization dashboard combining all findings

### 6. Deployment
- Jupyter notebook with reproducible analysis
- Stakeholder-friendly communication of findings
- Blog post for broader audience (link above)
- Documentation of limitations and future improvements

### System Requirements

- **Memory:** Minimum 4GB RAM (8GB recommended)
- **Storage:** ~500MB for datasets and outputs
- **OS:** Windows, macOS, or Linux

## Contributing

Contributions are welcome! This project is part of a learning exercise, but suggestions for improvements are appreciated.

### How to Contribute

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Make your changes and add tests if applicable
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Create a Pull Request

### Areas for Contribution

- **Data Collection:** Adding more recent datasets or additional cities
- **Feature Engineering:** Developing new predictive features
- **Modeling:** Implementing advanced algorithms (XGBoost, neural networks)
- **Visualization:** Creating interactive dashboards with Plotly/Dash
- **Documentation:** Improving code comments and documentation

## License

This project is distributed under the **MIT License**. See `LICENSE` file for more information.

**Dataset License:** Airbnb data is subject to [Inside Airbnb's license terms](http://insideairbnb.com/data-policies.html).

## Acknowledgments

- **Udacity** - For providing the Data Science Nanodegree curriculum and project framework
- **Inside Airbnb** - For making the datasets publicly available
- **scikit-learn community** - For the excellent machine learning library and documentation
- **CRISP-DM methodology** - For providing a structured approach to data mining projects

## Project History

This project was created in 2025 as part of the Udacity Data Science Nanodegree program. It demonstrates proficiency in:

- End-to-end data science project execution
- Machine learning model development and evaluation
- Statistical analysis and interpretation
- Data visualization and storytelling
- Stakeholder communication
- Python programming best practices (PEP8, DRY principles)

## Links

- **Repository:** https://github.com/iiPlayxX/udacity_datascience_proj_1
- **Blog Post:** https://medium.com/@vibrant_mandarin_porpoise_38/ai-data-scientists-guide-to-airbnb-pricing-what-really-drives-earnings-in-boston-vs-seattle-6ca4b6693ed5

## Author

**iiPlayxX**  
Udacity Data Science Nanodegree Student

---

*Last Updated: October 23, 2025*