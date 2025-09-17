# Currency Converter — API Bug vs Fix

## How to run the project
  1. In CMD: python -m http.server 8000
  2. On Browser: http://localhost:8000/index.html
## Challenge Statement
This project addresses a common **"Base Currency Assumption"** bug in currency converters.

**Reference Source:** [ExchangeRate API – Pair Conversion Requests](https://www.exchangerate-api.com/docs/pair-conversion-requests)

**Problem:**  
Many implementations assume that the API's **base currency** is the same as the user-selected "From" currency.  
APIs return rates relative to a fixed base (e.g., USD or EUR). If `fromCurrency ≠ baseCurrency`, directly multiplying:
```js
converted = amount * rates[to];
Submitted Current Working API
<img width="1887" height="758" alt="image" src="https://github.com/user-attachments/assets/41ee97e9-6201-40e8-94b1-64eb5f96bb73" />

