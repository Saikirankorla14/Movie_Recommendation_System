🔍 Overview
This project implements a simple movie/book recommendation system using collaborative filtering via the Surprise library in Python.

Recommendation systems suggest items to users based on their preferences. This project demonstrates a user-based and item-based collaborative filtering approach to predict how a user might rate an unseen item, and recommend top items accordingly.
⚙️ Technologies Used
- Python 3.8+
- Surprise Library
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook
🗂 Dataset
The system uses the popular MovieLens 100K dataset, containing:
- 100,000 ratings
- 943 users
- 1,682 movies

Alternatively, it can work with any dataset in the format: userId, itemId, rating.
📦 Installation
Run the following command to install dependencies:
pip install scikit-surprise pandas matplotlib seaborn
🚀 How to Run
1. Clone the repo:
   git clone https://github.com/your-username/recommendation-system.git
   cd recommendation-system

2. Run the notebook:
   jupyter notebook Recommendation_System.ipynb
📊 Visualizations
1. 🔎 Model Evaluation Metrics
We use standard evaluation metrics to assess performance:
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)

Example values:
RMSE: 0.89
MAE: 0.70

Example code:
from surprise import accuracy
accuracy.rmse(predictions)
accuracy.mae(predictions)
2. ⭐ Top Recommendations for a User
We generate top N recommendations for a given user based on predicted ratings.
![Top_Recommendation](https://github.com/user-attachments/assets/de63395c-67ec-425a-a27e-aecab573bd7c)

3. 📈 Predicted vs. Actual Ratings
We compare predicted ratings against actual ratings to evaluate accuracy.
![PredictedVsActual](https://github.com/user-attachments/assets/4fb6df0c-bf7e-49ad-a435-24529ad4f18b)

💡 Key Features
- Train/test split
- Evaluation with RMSE & MAE
- Recommend top N items for any user
- Visual comparison of predicted vs actual ratings
