🛍️ Customer Segmentation

Groups mall customers into segments using K-Means clustering and PCA, with a Streamlit app that predicts the segment of a new customer. Built as part of my AI/ML learning journey.

🛠️ Tech Stack
Python
Pandas, NumPy
Scikit-learn (KMeans, PCA, StandardScaler)
Matplotlib, Seaborn
Streamlit

📊 What This Project Does
Explores the Mall Customers dataset (200 customers)
Scales Annual Income and Spending Score
Finds the best number of clusters using the Elbow method and Silhouette score
Trains a K-Means model with 5 clusters (silhouette score 0.555)
Names each segment in business-friendly terms
Uses PCA to view Age, Income and Spending together in 2D
Streamlit app: enter income and spending, get the customer's segment and a marketing tip

📈 Customer Segments Found
Segment	Customers	Avg Age	Avg Income (k$)	Avg Spending
Average income - Average spending	81	42.7	55.3	49.5
High income - High spending (Target)	39	32.7	86.5	82.1
High income - Low spending (Careful)	35	41.1	88.2	17.1
Low income - High spending (Impulsive)	22	25.3	25.7	79.4
Low income - Low spending (Sensible)	23	45.2	26.3	20.9

Customer Segments Elbow and Silhouette PCA

💡 Key Findings
5 clusters gave the best silhouette score (0.555)
The "High income - High spending" group (39 customers, avg age about 33) is the best target for premium offers
The "High income - Low spending" group (35 customers) earns a lot but spends little, so personalised offers could unlock more sales
The "Low income - High spending" group is the youngest (avg age about 25)
PCA keeps 78% of the information from Age, Income and Spending in just 2 dimensions


## 🚀 How to Run
```bash
pip install -r requirements.txt
jupyter notebook customer_segmentation.ipynb
```

# Run the app
streamlit run app.py

📁 Project Files
customer_segmentation.ipynb : full analysis (EDA, K-Means, PCA)
app.py : Streamlit app
Mall_Customers.csv : dataset
customers_with_segments.csv : output with the segment of every customer
requirements.txt : libraries needed
*.png : result charts

📚 Dataset
Mall Customers dataset (Kaggle)

👤 Author

Shanti | Aspiring AI/ML Developer | Open to Work
