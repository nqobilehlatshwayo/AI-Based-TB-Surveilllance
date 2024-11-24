# AI-Based TB Surveillance in South Africa using Google Trends

This repository contains the research implementation and findings for AI-based surveillance of Tuberculosis in South Africa using Google Trends data, completed as part of an Honours research project at the University of the Witwatersrand.

## Repository Structure

```
├── LICENSE
├── README.md
├── .gitignore
├── requirements.txt
├── data/
│   ├── merged_tb_data.csv     # Merged Google Trends data and TB surveillance data from NICD
│   └── README.md         # Data documentation
├── notebooks/
│   └── tb_final_models.ipynb  # Main analysis notebook
└── results/          # Generated plots and visualizations
```

## Project Overview

This research investigates the potential of integrating Google Trends data with Machine Learning approaches for forecasting TB incidence in South Africa. The study implements and compares four ML models:

- Partial Least Squares (PLS) regression
- LASSO regression
- Support Vector Machine (SVM)
- Long Short-Term Memory (LSTM) networks

### Key Findings

The PLS model demonstrated superior performance with:
- R² value: 0.889
- RMSE: 7.173
- MAE: 5.704

This outperformed more complex approaches, suggesting that simpler linear models may be more effective for TB surveillance in South Africa.

## Data Sources

- **TB Incidence Data**: National Institute for Communicable Diseases (NICD)
- **Google Trends Data**: Search volume data for 27 TB-related terms
- **Time Period**: 2012-2021 (40 quarters)

## Getting Started

### Prerequisites
- Python 3.8+
- Required packages listed in `requirements.txt`

### Installation
1. Clone this repository
```bash
git clone https://github.com/nqobilehlatshwayo/AI-Based-TB-Surveilllance.git
cd AI-Based-TB-Surveillance
```

2. Create and activate a virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate.bat
```

3. Install required packages
```bash
pip install -r requirements.txt
```

### Running the Analysis

The complete analysis is contained in `notebooks/tb_final_models.ipynb`. This notebook includes:
1. Data preprocessing
2. Feature selection and correlation analysis
3. Model implementation:
   - PLS regression
   - LASSO regression
   - SVM
   - LSTM
4. Performance evaluation and visualization

## Model Performance Summary
| Model | MSE | RMSE | MAE | R² |
|-------|-----|------|-----|-----|
| PLS | 51.450 | 7.173 | 5.704 | 0.889 |
| LASSO | 93.029 | 9.645 | 7.123 | 0.800 |
| SVM | 144.193 | 12.008 | 9.174 | 0.696 |
| LSTM | 202.279 | 14.223 | 12.211 | 0.573 |

## Future Work Recommendations

1. Expansion to include social media data sources
2. Integration of multilingual Natural Language Processing
3. Development of ensemble approaches combining multiple data sources
4. Real-time implementation for early warning system

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author
- Nqobile Hlatshwayo
- Honours in Computer Science
- University of the Witwatersrand, Johannesburg

## Supervisor
- Dr. Seun Olukanmi

## Acknowledgments
- University of the Witwatersrand, Johannesburg
- National Institute for Communicable Diseases (NICD) for data access
