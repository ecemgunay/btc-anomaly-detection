# 📊 BTC Price Anomaly Detection Using Z-Score

![Anomaly Detection Chart](./btc_anomaly_chart.jpg)

This project demonstrates a simple statistical approach to detect anomalies in Bitcoin (BTC) closing prices using the **Z-score** method. The analysis is performed in Python with `pandas`, `NumPy`, and `matplotlib`, and visualizes the abnormal price movements based on statistical thresholds.

---

## 🔍 Objective

To identify statistically significant deviations in daily BTC closing prices and visualize the results to gain quick insights about unusual market behavior.

---

## 📁 Project Structure

```
btc-anomaly-detection/
├── btc_anomaly_detection.ipynb   # Jupyter notebook with full analysis
├── data/
│   └── btc_price_data.csv        # Price data (simulated or real)
├── README.md                     # Project documentation
└── requirements.txt              # Python dependencies (optional)
```

---

## 📊 Visualization Example

The chart below shows BTC price over time with red dots marking anomalies (Z-score > 2):

> _(You can include the chart here later as a PNG or let GitHub render the notebook.)_

---

## ⚙️ How It Works

1. Load BTC price data from CSV
2. Calculate Z-scores for each price
3. Mark all values where |Z-score| > 2 as anomalies
4. Plot and interpret

```python
df['Z-Score'] = (df['Price'] - df['Price'].mean()) / df['Price'].std()
df['Anomaly'] = np.abs(df['Z-Score']) > 2
```

---

## 📖 Related Blog Post

📎 You can read the full explanation on Medium here:  
👉 [Coming soon – insert your Medium link here]

---

## 🧠 Key Takeaways

- Simple statistical tools like Z-score can help flag unusual market behavior.
- This approach is useful for **alert systems**, **risk monitoring**, and **data quality checks** in crypto platforms.

---

## 📦 Requirements

```text
pandas
numpy
matplotlib
```

> You can install dependencies with:
```bash
pip install -r requirements.txt
```

---

## 📝 License

This project is open source and available under the MIT License.