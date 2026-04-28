# turbofan-predictive-maintenance

A machine learning project that predicts the Remaining Useful Life (RUL) 
of aircraft turbofan engines using NASA's CMAPSS dataset.

## Problem Statement
Aircraft engine failures are costly and dangerous. This project builds a 
predictive maintenance model that estimates how many cycles an engine has 
left before failure — enabling early intervention before breakdowns occur.

## Dataset
- **Source:** NASA CMAPSS (Commercial Modular Aero-Propulsion System Simulation)
- **Subset:** FD001 — 158 engines, 20,631 sensor readings
- **Features:** 3 operational settings + 21 sensor measurements per cycle

## Approach
1. Loaded and cleaned raw sensor data
2. Calculated Remaining Useful Life (RUL) for each engine
3. Removed low-variance sensors that don't contribute to prediction
4. Trained a Random Forest Regressor model
5. Evaluated model performance

## Results
| Metric | Score |
|---|---|
| R² Score | 0.6257 |
| Mean Absolute Error | 29.59 cycles |

## Technologies Used
- Python 3.13
- Pandas, NumPy
- Scikit-learn (Random Forest)
- Matplotlib, Seaborn

## Real World Relevance
Predictive maintenance using sensor data is actively used in aerospace 
and industrial engineering. This project mirrors work done at companies 
like GE Aerospace and BEML for engine health monitoring.

## Author
S Adhithya — [LinkedIn](https://www.linkedin.com/in/s-adhithya-41a560379)
