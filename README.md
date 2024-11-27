# Market Mix Models Using Advanced Regression Methods

## Project Description
This project focuses on developing **Market Mix Models (MMM)** to evaluate and optimize the contributions of various marketing channels (e.g., TV, radio, digital ads) to overall sales or revenue. By employing advanced regression techniques and hyperparameter tuning, the model provides actionable insights for budget allocation to maximize marketing impact.

---

## Folder Structure
```
MarketMixModeling/
│
├── data/
│   └── marketing_data.csv   # Input data with channel-wise spends and sales/revenue
│
├── scripts/
│   ├── data_preprocessing.py   # Data cleaning and preprocessing
│   ├── regression_model.py     # Model building and optimization
│   ├── evaluation.py           # Model evaluation and insights
│
├── outputs/
│   └── model_results.csv       # Contribution of each channel
│
├── README.md
└── requirements.txt
```

---

## Setup Instructions

1. **Clone this repository:**
   ```bash
   git clone <repository_link>
   cd MarketMixModeling
   ```

2. **Install the required libraries:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Place your dataset in the `data/` folder.**  
   The dataset should have the following structure:
   ```
   TV_Spend, Radio_Spend, Digital_Spend, Other_Spend, Sales
   200, 100, 300, 50, 800
   ```

4. **Run the project:**
   - Preprocess data:
     ```bash
     python scripts/data_preprocessing.py
     ```
   - Train the model:
     ```bash
     python scripts/regression_model.py
     ```
   - Evaluate the results:
     ```bash
     python scripts/evaluation.py
     ```

---

## Key Features
- **Quantify Channel Contributions**: Understand how much each marketing channel contributes to sales.
- **Regression Optimization**: Uses advanced regression techniques (e.g., Ridge, Lasso) with hyperparameter tuning.
- **Actionable Insights**: Recommendations for optimal budget allocation.

---

## Outputs
1. **Mean Squared Error (MSE)** and **R² Score**: Evaluates model performance.
2. **Channel Contribution Analysis**: A CSV file in `outputs/model_results.csv` showing the percentage contribution of each marketing channel.

---

## Requirements
- Python 3.7+
- pandas
- scikit-learn
- joblib

Install all dependencies using:
```bash
pip install -r requirements.txt
```

---

## Example Results
An example of channel contribution percentages:
| Channel       | Contribution (%) |
|---------------|------------------|
| TV_Spend      | 45.3            |
| Radio_Spend   | 25.6            |
| Digital_Spend | 20.7            |
| Other_Spend   | 8.4             |

---

## License
This project is licensed under the MIT License.

---
