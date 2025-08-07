# RedBus Demand Forecasting Model

This project was built as part of the RedBus Hackathon to forecast the number of seats booked 15 days prior to a journey date. The model uses historical booking and search data and is evaluated based on RMSE (Root Mean Squared Error).

The aim is to assist in **demand planning and inventory optimization** by accurately predicting bus occupancy using machine learning.

---

## 🚀 Features

- Predicts bus seat bookings 15 days before journey date
- Uses engineered features like holidays, routes, and seat-to-search ratios
- Built using XGBoost with tuning for RMSE optimization
- Developed entirely in **Google Colab**

---

## 🧠 Model

- **Algorithm Used**: XGBoost Regressor
- **Evaluation Metric**: RMSE
- **Target Variable**: Total seats booked 15 days before journey date

---

## 📁 Project Structure

redbus-bus-demand-forecasting/
│
├── redbus_model.ipynb        # Main Jupyter Notebook
├── README.md                 # Project documentation
│
├── input/                    # Input data
│   ├── train.csv             # Historical booking/search data
│   └── test.csv              # Test data for prediction
│
├── output/                   # Output directory
│   └── submission.csv        # Final predictions


yaml
Copy
Edit

---

## 📊 Input Features (examples)

- `source`, `destination`, `bus_type`, `route`
- `journey_date`, `booking_date`, `search_date`
- `is_weekend`, `is_holiday`, `is_peak_season`
- `seat_to_search_ratio`

---

## 📝 How to Use

1. Open the notebook in Google Colab (recommended)
2. Upload the datasets (`train.csv`, `test.csv`) when prompted
3. Run the cells sequentially to train the model and generate predictions

---

## 📌 Notes

- Developed using **Google Colab**
- You may need to upload input files manually or mount Google Drive
- Data files are not included due to size/privacy — replace with your own

---

## 🔧 Requirements

- Python 3.x
- pandas, numpy, xgboost, scikit-learn, matplotlib, seaborn

Install dependencies (if working locally):

```bash
pip install pandas numpy xgboost scikit-learn matplotlib seaborn
👩‍💻 Author
Supreet Kaur

