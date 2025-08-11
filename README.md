# 🏠 Housing Price Predictor

This project predicts housing prices using **Linear Regression** on the Boston Housing Dataset (or similar housing data). 
It analyzes key features such as crime rate, number of rooms, and location to estimate the market value of houses.

---

## 📂 Project Structure
```
├── Housing Price Predictor.ipynb   # Jupyter Notebook with code
├── HousingData.csv                 # Dataset file
├── model.pkl                       # Saved trained model using pickle
├── README.md                       # Project documentation
└── requirements.txt                # Python dependencies
```

---

## 📊 Dataset
- **Name:** Boston Housing Dataset (or compatible)
- **Source:** [Boston Housing Dataset on Kaggle](https://www.kaggle.com/datasets/altavish/boston-housing-dataset)
- **Target Column:** `MEDV` (Median value of owner-occupied homes in $1000's)
- **Features:** Includes variables such as crime rate, number of rooms, property age, and accessibility to highways.

---

## 🚀 How to Run

1️⃣ **Clone the repository**  
```bash
git clone https://github.com/your-username/housing-price-predictor.git
cd housing-price-predictor
```

2️⃣ **Install dependencies**  
```bash
pip install -r requirements.txt
```

3️⃣ **Run the notebook**  
```bash
jupyter notebook "Housing Price Predictor.ipynb"
```

4️⃣ **Use the Pickle model**  
```python
import pickle

# Load model
with open("model.pkl", "rb") as file:
    model = pickle.load(file)

# Example prediction
prediction = model.predict([[value1, value2, ..., valueN]])
print("Predicted Price:", prediction)
```

---

## 💾 Saving the Model with Pickle
In the notebook, after training the model, you can save it like this:
```python
import pickle

with open("model.pkl", "wb") as file:
    pickle.dump(model, file)
```

---

## 📈 Output Example
After running the notebook, you will see:
- **Mean Squared Error** of the predictions
- **Scatter plot** comparing actual vs predicted prices

---

## 🛠 Requirements
- Python 3.x
- pandas
- numpy
- matplotlib
- scikit-learn

---

## 📌 Future Improvements
- Try advanced models like Random Forest or Gradient Boosting
- Implement a web app with Streamlit for interactive predictions
- Add hyperparameter tuning for better accuracy

---

## 👩‍💻 Author
Shalini Saurav  
BTech Student | Data Science & Machine Learning Enthusiast
