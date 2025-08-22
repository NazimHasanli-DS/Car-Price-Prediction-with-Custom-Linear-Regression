# Car-Price-Prediction-with-Custom-Linear-Regression

## 📌 Layihə haqqında
Bu layihə **Turbo.az** datasetindən istifadə edərək maşın qiymətlərini (`Qiymət`) proqnozlaşdırmaq üçün **Linear Regression modelini sıfırdan (scratch)** qurur. 
Model **Gradient Descent** alqoritmi ilə öyrədilir və nəticələr sınaqdan keçirilir.

## 🎯 Məqsəd
- Data cleaning (Qiymət və Yürüş dəyişənlərinin təmizlənməsi)
- Öz `LinearRegression` sinfini qurmaq
- Gradient descent ilə parametrləri öyrətmək
- Maşın qiymətini proqnozlaşdırmaq

## ⚙️ Texnologiyalar
- Python (pandas, numpy)

## 🚀 Addımlar
1. Dataset təmizlənir (`Qiymət` → float, `$` → AZN, `Yürüş` → integer).
2. Öz `LinearRegression` sinfi yaradılır:
   - `fit()` → gradient descent
   - `predict()` → yeni qiymət proqnozu
3. Model test olunur:
   ```python
   m.predict([2020, 23420])
   # Çıxış: ~60670 AZN
