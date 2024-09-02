# Publication 

This project is submitted to the 15th Vietnam Economist Annual Meeting (VEAM 2024), soon published on the conference proceeding site as "[CLAM: A Synergistic Deep Learning Model for Multi-Step Stock Trend Forecasting](https://drive.google.com/file/d/1ckaukHiU5otFOi-PDuF0FQT-4r_uJUGa/view?usp=sharing)". 

**Re-produce CLAM in LightningAI:** 
>https://lightning.ai/thequantscientist/studios/clam-a-simple-swing-trading-indicator
## Introduction 

Our team presents a cutting-edge approach that leverages the strengths of Convolutional Neural Networks (CNNs), Long Short-Term Memory networks (LSTMs), and Attention Mechanisms (AM) to enhance the accuracy of stock market predictions. By integrating these powerful techniques, our CLAM model addresses the limitations of traditional forecasting methods, offering a more comprehensive understanding of market dynamics.

## Project Overview

The study presents the CLAM model, a hybrid deep learning architecture combining Convolutional Neural Networks (CNNs), Long Short-Term Memory (LSTM) networks, and an Attention Mechanism (AM), designed for multi-step stock price trend forecasting. The model was tested on OHLCV data from four prominent stocks over a 20-year period, focusing on the "Close" prices as the target feature. CLAM demonstrated superior performance compared to traditional models like CNN, LSTM, and their hybrids, achieving significant reductions in both Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE), with up to 91.8% improvement in MAE and 89.4% in RMSE on validation sets. The model's trend forecasting accuracy averaged 75%, effectively capturing market momentum and predicting consecutive trends, especially during volatile periods. Despite minor inconsistencies in some predictions, CLAM's robust architecture and sophisticated regularization techniques underscore its potential for practical financial applications, offering a promising framework for accurate time series forecasting in complex, high-stakes environments.

## Features

- **Integration of CNN, LSTM, and Attention Mechanisms:** This combination leverages CNN's feature extraction capabilities, LSTM's sequence learning, and the dynamic focusing ability of Attention Mechanisms, creating a powerful tool for market forecasting.

- **Attention Mechanisms for Dynamic Focus:** The Attention Mechanisms embedded in the model enhance its ability to prioritize the most relevant temporal and spatial features, improving prediction accuracy.

- **Customizable Neural Architecture:** The model architecture is designed to be flexible, allowing for easy customization and fine-tuning to suit various stock datasets and forecasting requirements.

- **Use of Time Series Split for Model Validation:** The application of TimeSeriesSplit for model validation respects the temporal order of the data, which is crucial for time series forecasting.

- **Early Stopping Mechanism:** Implementation of an early stopping mechanism to prevent overfitting, improving the generalizability of the model.

- **Efficient Data Preprocessing and Scaling:** The detailed preprocessing steps, including scaling of features and target variables, ensure that the model receives data in an optimal format for learning.
  

## Technologies Used

- **Pandas:** Used for data manipulation and analysis, particularly for loading the stock price data from CSV files and preprocessing it for the model.

- **NumPy:** Utilized for numerical computing, especially in handling arrays and performing calculations related to the model's input features.

- **Scikit-learn (sklearn):** This library is employed for preprocessing capabilities (e.g., MinMaxScaler for feature scaling) and for splitting the dataset into training and validation sets (TimeSeriesSplit), as well as for evaluating the model's performance using metrics like MAE and RMSE.

- **Keras/TensorFlow:** These deep learning frameworks are used to define and train the CLAM model, including the CNN layers, LSTM layers, and Attention Mechanisms. They provide the infrastructure for model training, including automatic differentiation to compute gradients and optimizers (e.g., Adam) for updating model parameters.

- **Matplotlib/Seaborn:** Used for visualizing the model's performance, including plotting error metrics and the progression of loss during training.

- **Copy:** A standard Python library used for deep copying model states, enabling the implementation of early stopping by keeping track of the best model weights during training.


## Getting Started

Follow the instructions in the subsequent sections to set up your environment, train the model with your dataset, and evaluate its performance on stock price forecasting tasks using evaluation metrics such as MAE and RMSE. This model has been tested on various datasets of prominent technology, financial, and pharmaceutical companies, demonstrating its capability to accurately capture market trends and fluctuations.
