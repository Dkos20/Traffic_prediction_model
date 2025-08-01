# 🚦 Predikcija gužve u prometu pomoću XGBoost algoritma

Ovaj projekt fokusiran je na predikciju **prometne gužve** koristeći algoritam **XGBoost**. Analiza i modeliranje provedeni su u okruženju Google Colab, a cilj je bio razviti model koji pouzdano predviđa prometnu zagušenost temeljem vremenskih i prometnih karakteristika.

---

## 📋 Opis projekta

Model koristi skup podataka koji uključuje vremenske i vremenski povezane značajke poput:
- `date_time` (datum i vrijeme)
- `is_holiday` (je li praznik)
- `weather_type` (tip vremena)
- `temperature`, `humidity`, `wind_speed`
- `avg_speed` (prosječna brzina prometa)
- `avg_volume` (prosječni prometni volumen)

Ciljna varijabla: `congestion` (stupanj gužve, kvantificiran)

---

## ⚙️ Korištene metode

1. 🧼 **Priprema podataka**
   - Pretvaranje datuma u značajke (`dan`, `sat`, `dan_u_tjednu`)
   - One-hot enkodiranje vremenskih uvjeta
   - Skaliranje numeričkih podataka (`MinMaxScaler`)

2. 📈 **Modeliranje**
   - `XGBoostRegressor` za regresijsku analizu
   - Evaluacija modela pomoću:
     - RMSE (Root Mean Squared Error)
     - MAE (Mean Absolute Error)
     - R² Score
   - 5-struka križna validacija (`KFold`)

---

## 🧠 Rezultati

Prosječne metrike nakon 5-struke validacije:
- **RMSE:** ~6.53
- **MAE:** ~5.03
- **R²:** ~0.72

Model pokazuje solidnu točnost i može se koristiti kao baza za buduće poboljšane sustave predikcije prometa.

---

## 🔧 Tehnologije

- 🐍 Python 3 (Google Colab)
- 📦 Pandas, NumPy
- 📊 Seaborn, Matplotlib
- 🧪 Scikit-learn
- ⚡ XGBoost

---

## ▶️ Pokretanje

Notebook je dostupan putem Google Colaba:  
📎 [Otvori u Colabu](https://colab.research.google.com/drive/1TRJDGhQju-BqhzLNmT8vi-rM4elUh6PK?usp=sharing)

