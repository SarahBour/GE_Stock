# 📈 GE Aerospace Stock Price Prediction

## 📌 Project Overview
This project utilizes historical stock price data of **GE Aerospace** from **January 2021 to February 14, 2025** to predict the **next day's opening price** using a **Bidirectional LSTM (BiLSTM) model**. The goal is to enhance forecasting accuracy by leveraging deep learning techniques.

## 🛠️ Technologies Used
- **Python** 🐍
- **TensorFlow/Keras** 🤖
- **Pandas & NumPy** 📊
- **Matplotlib** 📉
- **Scikit-learn** 🏆

## 📂 Dataset
- **Source:** [Dataset source](https://www.investing.com/equities/general-electric-historical-data)
- **Features used:** Opening price (scaled), additional technical indicators can be added for improvement.

## 🏗️ Model Architecture
- **BiLSTM Layers:** Multiple stacked layers for better learning of sequential dependencies.
- **Dropout Layers:** Regularization to prevent overfitting.
- **Dense Layer:** Final output layer to predict the next opening price.

```python
model = Sequential()
model.add(Bidirectional(LSTM(units= 128, return_sequences=True), input_shape=(X_train.shape[1], 1)))
model.add(Bidirectional(LSTM(units=128)))
model.add(Dense(units=1))
```

## 📊 Results & Performance
- The model captures **overall trends** well but may require **fine-tuning** to improve short-term price movement accuracy.
- Potential improvements include **adding more features** (trading volume, moving averages) and **hyperparameter tuning**.

## 🚀 How to Use
1. Clone this repository.
2. Install required dependencies.
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Train the model and visualize the predictions.

## 🔥 Future Improvements
- 📌 **Feature Engineering:** Incorporate trading volume, technical indicators, and external market sentiment.
- 🎯 **Hyperparameter Tuning:** Optimize LSTM layers, batch size, and learning rate.

## 📬 Contact
For any questions or contributions, feel free to reach out! 🚀

