# Crude Oil Price Forecasting using Deep Learning

This project presents a comparative study of advanced deep learning architectures for forecasting crude oil prices under volatile market conditions. The models are trained on daily crude oil price data and evaluated using multiple performance metrics.

## Overview

Crude oil prices are highly influenced by geopolitical events, supply-demand dynamics, and economic factors, making accurate forecasting challenging. This project explores three different deep learning approaches to capture various patterns in time-series data:

- CBAM-CNN (Attention-based CNN)
- Multi-Channel CNN (Multi-scale feature extraction)
- Graph Convolutional Network (GCN) (Relational modeling)

The goal is to compare their performance and understand whether increased model complexity leads to better forecasting accuracy.

---

## Models Used

### 1. CBAM-CNN
An enhanced convolutional neural network integrated with an attention mechanism to focus on important features in the data.

### 2. Multi-Channel CNN
A CNN architecture with parallel convolutional paths to capture patterns at different time scales.

### 3. Graph Convolutional Network (GCN)
A graph-based approach that models relationships between time steps to capture non-local dependencies.

---

## Dataset

- Source: Investing.com  
- Type: Crude Oil Price Data  
- Frequency: Daily  
- Duration: 2 years (from April 1, 2024)  

---

## Methodology

- Data preprocessing and normalization
- Sliding window approach for sequence generation
- Model training using TensorFlow / PyTorch
- Evaluation using standard regression metrics

---

## Results

| Model                | MAE (USD/bbl) | RMSE (USD/bbl) | MAPE (%) | R²     |
|---------------------|--------------|---------------|----------|--------|
| GCN                 | 1.95         | 3.00          | 2.54     | 0.9589 |
| CBAM-CNN            | 1.95         | 2.99          | 2.55     | 0.9592 |
| Multi-Channel CNN   | 1.95         | 3.00          | 2.53     | 0.9590 |

All models achieved similar performance, indicating that architectural complexity does not significantly impact short-term forecasting accuracy under limited data conditions.

---

## Visualizations

The project includes:
- Training & validation loss curves
- Predicted vs actual price comparison
- Residual error analysis
- Scatter plots for model evaluation

---

## Key Insights

- All architectures show strong trend prediction capability
- Attention and graph-based models perform comparably to CNN variants
- Data characteristics play a more significant role than model complexity

---

## Future Work

- Incorporating external features (news sentiment, geopolitical data)
- Exploring hybrid architectures (GCN + Attention)
- Extending dataset for long-term forecasting

---

## Tech Stack

- Python
- TensorFlow / PyTorch
- NumPy, Pandas
- Matplotlib / Seaborn

---

## License

This project is for academic and research purposes.

---

## Author

Ameesh Rawat  