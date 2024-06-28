# Sales-Forcast-for-Olist-Brazilian-E-commerce

## Customer Segmentation
| K-Means Cluster | Recency | Frequency | Monetary | Count | Customer Description    |
|-----------------|---------|-----------|----------|-------|-------------------------|
| 0               | 128.2   | 1.0       | 113.3    | 50997 | New Low-Spenders        |
| 1               | 387.7   | 1.0       | 114.2    | 37399 | Hibernating Low-Spenders|
| 2               | 219.9   | 2.1       | 243.2    | 2774  | Loyalists               |
| 3               | 237.2   | 1.0       | 1142.2   | 2188  | Big Spenders            |

![k-mean](images\kmeanscatter.png)

## Sales Forecast
| Model                               | Mape   |
|-------------------------------------|--------|
| SARIMA(1,1,1)(0,1,1)(7)             | 68.99  |
| SARIMA(1,1,2)(0,1,1)(7) with Holiday| 65.66  |
| Basic FB Prophet                    | 75.24  |
| Basic FB Prophet with holiday       | 75.79  |
| **Tunned FB Prophet with holiday**      | **49.24**  |
| Basic XGboost with holiday          | 51.29  |
| Tunned XGboost with holiday         | 45.18  |

![fore-cast](images\forecast.png)
