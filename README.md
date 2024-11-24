# AI-Based TB Surveillance in South Africa using Google Trends 🔬

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Research](https://img.shields.io/badge/Research-Honours-purple.svg)](https://www.wits.ac.za/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.13.0-orange.svg)](https://tensorflow.org)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.2.2-red.svg)](https://scikit-learn.org)

## 📋 Table of Contents
- [Overview](#overview)
- [Key Findings](#key-findings)
- [Repository Structure](#repository-structure)
- [Data Sources](#data-sources)
- [Getting Started](#getting-started)
- [Model Performance](#model-performance)
- [Future Work](#future-work)
- [Contributors](#contributors)

## 🔍 Overview

Tuberculosis (TB) remains a critical public health issue globally, with the WHO Global TB Report 2024 confirming TB as the world's deadliest infectious disease. South Africa has one of the highest TB burdens globally, reporting an estimated 56,000 TB-related deaths in 2023.

### 🎯 Research Objectives
This research investigates the potential of integrating Google Trends data with Machine Learning approaches to enhance TB surveillance in South Africa, addressing key limitations of traditional surveillance:
- Reporting delays
- Incomplete case capture
- Poor data quality

### 🤖 Models Implemented
- Partial Least Squares (PLS) regression
- LASSO regression
- Support Vector Machine (SVM)
- Long Short-Term Memory (LSTM) networks

## 📊 Key Findings

The PLS model demonstrated superior performance:

<table>
  <tr>
    <td><b>R² Value</b></td>
    <td><b>RMSE</b></td>
    <td><b>MAE</b></td>
  </tr>
  <tr>
    <td>0.889</td>
    <td>7.173</td>
    <td>5.704</td>
  </tr>
</table>

> 💡 **Key Insight**: Simpler linear models outperformed complex deep learning approaches for TB surveillance in South Africa.

## 📁 Repository Structure
```
├── LICENSE
├── README.md
├── .gitignore
├── requirements.txt
├── data/
│   ├── merged_tb_data.csv     # Merged surveillance data
│   └── README.md              # Data documentation
├── notebooks/
│   └── tb_final_models.ipynb  # Main analysis notebook
└── results/                   # Generated visualizations
```

## 📚 Data Sources

| Source | Description | Time Period |
|--------|-------------|-------------|
| NICD | TB Incidence Data | 2012-2021 |
| Google Trends | 27 TB-related search terms | 2012-2021 (40 quarters) |

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Required packages from `requirements.txt`

### Installation

1. Clone the repository
```bash
git clone https://github.com/nqobilehlatshwayo/AI-Based-TB-Surveilllance.git
cd AI-Based-TB-Surveillance
```

2. Set up environment
```bash
python -m venv venv
.\venv\Scripts\activate  # Windows
source venv/bin/activate # Linux/Mac
```

3. Install dependencies
```bash
pip install -r requirements.txt
```

### 📓 Running the Analysis

The complete analysis workflow is in `notebooks/tb_final_models.ipynb`:

1. 🔧 Data preprocessing
2. 🎯 Feature selection and correlation analysis
3. 🤖 Model implementation
4. 📊 Performance evaluation

## 📈 Model Performance

| Model | MSE | RMSE | MAE | R² |
|:------|:---:|:----:|:---:|:--:|
| **PLS** | 51.450 | **7.173** | **5.704** | **0.889** |
| LASSO | 93.029 | 9.645 | 7.123 | 0.800 |
| SVM | 144.193 | 12.008 | 9.174 | 0.696 |
| LSTM | 202.279 | 14.223 | 12.211 | 0.573 |

## 🔮 Future Work

1. 📱 **Data Integration**
   - Incorporate social media data sources
   - Develop real-time monitoring capabilities

2. 🌐 **Language Processing**
   - Implement multilingual NLP
   - Enhance feature extraction

3. 🤝 **Ensemble Approaches**
   - Combine multiple data sources
   - Develop hybrid models

4. ⚡ **System Implementation**
   - Deploy real-time early warning system
   - Integrate with existing surveillance

## 👥 Contributors

### Author
<img src="https://img.shields.io/badge/Researcher-Nqobile%20Hlatshwayo-blue">
- Honours in Computer Science
- University of the Witwatersrand, Johannesburg

### Supervisor
<img src="https://img.shields.io/badge/Supervisor-Dr.%20Seun%20Olukanmi-green">

## 🙏 Acknowledgments
- University of the Witwatersrand, Johannesburg
- National Institute for Communicable Diseases (NICD)

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
<p align="center">
  Made with ❤️ at the University of the Witwatersrand
</p>
