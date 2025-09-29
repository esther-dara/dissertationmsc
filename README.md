# dissertationmsc
**Fairness in NHS Readmissions Prediction with FAIM**

This repository contains the code and outputs for my MSc dissertation project, which replicated and extended the Fairness-Aware Interpretable Modelling (FAIM) framework (Liu et al., 2023) using NHS readmissions data (2011–2024).

The project investigates whether AI models can balance predictive accuracy with fairness across sensitive groups (Gender, Age), contributing to SDG 3 (Good Health & Well-being) and SDG 10 (Reduced Inequalities).

📂 Repository Structure

data/  
notebooks/ → Jupyter/Colab notebooks with executed code and outputs

src/ → Clean, modular Python scripts (preprocessing, training, fairness evaluation, plots)

results/ → Tables, fairness metrics, and visualisations

original_code/ → Link/reference to FAIM’s original repository

requirements.txt → Python dependencies

LICENSE → MIT open-source licence


⚙️ How to Run

Clone this repo

Install requirements:

pip install -r requirements.txt

Follow pipeline:

preprocessing.py → clean & encode NHS data

train_faim.py → generate nearly-optimal models

fairness_eval.py → evaluate with fairlearn (Equalised Odds, Equal Opportunity, Predictive Parity, etc.)

test_eval.py → final test set evaluation


📊 Key Contributions

Replicated FAIM on NHS data (first application beyond US datasets)

Extended fairness evaluation with Predictive Parity using fairlearn

Identified that Equalised Odds implied parity, but disparities surfaced in other metrics

Demonstrated practical reproducibility challenges and methodological adaptations


📖 Citation

If you use this code, please cite:

Liu, Y. et al. (2023). Fairness-Aware Interpretable Modeling for Healthcare AI
