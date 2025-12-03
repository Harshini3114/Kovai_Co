Understood. Here is your content **exactly as given, nothing added, nothing removed**, only formatted properly and professionally:

---

## **Kovai Co**

### **Problem Statement**

The given dataset consists of different travel modes taken on different days and we need to predict the values for the upcoming days.

---

## **SARIMAX Model – Workflow**

* First data is cleaned and processed and some trends are obtained so that outliers can be minimised.
* Then we find parameters for the SARIMAX model.
* Model is built.
* Values are forecast.
* Error is calculated and plotted.

---

## **Insights Gained**

### **Top transport modes on weekdays:**

![Weekdays](weekday.png)

### **Top transport on weekends:**

![Weekends](weekend.png)

### **Top transport on holidays:**

![Holidays](weekday.png)

---

## **SARIMAX Parameters**

* **p** → number of past values used (AR lags)
* **d** → differencing to remove trend and make data stationary
* **q** → number of past errors used (MA lags)

### **seasonal_order = (P, D, Q, m)**

* **P** → seasonal AR lags
* **D** → seasonal differencing to remove repeating season trend
* **Q** → seasonal MA lags
* **m** → length of season depending on data frequency

---

## **Prophet Model – Parameters**

* **yearly_seasonality** → learns patterns that repeat every year
* **weekly_seasonality** → learns every-7-day patterns
* **daily_seasonality** → learns 24-hour patterns

### **seasonality_mode**

* **additive** → season added to trend

* **multiplicative** → season multiplied with trend

* **n_changepoints** → number of places trend can change direction

* **changepoint_prior_scale**

  * higher → trend becomes more flexible
  * too high → overfits
  * too low → underfits

* **seasonality_prior_scale** → strength of seasonality fitting

* **interval_width** → confidence interval range (ex: 0.95 = 95%)

---

## **Model Suitability**

* Model for trend + seasonality forecasting.
* Best suited for:

  * data with multiple trend changes
  * data with strong seasonal patterns

---

## **Model Comparison**

Two models are compared for the **Peak Services Column** and better prediction is obtained with the **SARIMAX model** with lower MSE, RMSE, MAE, and MAPE.

---
