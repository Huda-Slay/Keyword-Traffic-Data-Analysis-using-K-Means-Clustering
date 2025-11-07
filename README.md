# Keyword-Traffic-Data-Analysis-using-K-Means-Clustering
This project focuses on analyzing keyword traffic data to identify meaningful clusters based on Keyword ID and Cost Per Click (CPC) values. Using K-Means Clustering, we segment keywords into groups with similar traffic and cost behavior — which can help in optimizing keyword strategies and understanding ad performance patterns.
The analysis was performed in Google Colab using Python’s data science libraries.


🧩 Objectives

To explore keyword traffic data and understand CPC distribution.
To determine the optimal number of clusters using the Elbow Method.
To apply K-Means Clustering and visualize the keyword groups.
To derive insights that differentiate high-cost, medium-cost, and low-cost keyword clusters.

⚙️ Tech Stack & Libraries

Python
NumPy – for numerical computation
Pandas – for data manipulation
Matplotlib & Seaborn – for data visualization
Scikit-learn – for machine learning (K-Means algorithm)
Google Colab – as the development environment

🧠 Project Workflow

1️⃣ Data Loading & Exploration

Loaded dataset into Pandas DataFrame.

Explored structure using .head(), .info(), and .describe() to understand data types, nulls, and summary stats.

2️⃣ Data Cleaning

Removed missing or invalid rows from selected features (Keyword_ID, CPC) for accurate clustering.

3️⃣ Feature Selection

Selected two key features:

Keyword_ID (represents unique keyword identifier)

CPC (Cost Per Click) (represents keyword bidding cost)

4️⃣ Elbow Method for Optimal Clusters

Computed inertia for cluster values from 1 to 14.

Plotted Number of Clusters vs Inertia to identify the “elbow point.”

The curve flattened around k=3, indicating 3 clusters as optimal.
(See Plot 1 – Elbow Curve)

5️⃣ K-Means Clustering

Implemented KMeans(n_clusters=3, random_state=42) from sklearn.

Fitted model on selected features and assigned cluster labels to each record.

6️⃣ Visualization

Visualized results with data points colored by their cluster and centroid locations.

Background regions show cluster decision boundaries.
(See Plot 2 – Cluster Decision Boundaries)

📊 Results & Insights

Cluster 1: Low CPC keywords — cost-efficient group.

Cluster 2: Moderate CPC keywords — balanced cost-performance group.

Cluster 3: High CPC keywords — premium group, fewer but costly clicks.

These clusters help in segmenting keyword strategies: focusing budget on high-return clusters while managing spend on low-impact ones. 

Elbow_plot.png
<img width="1010" height="394" alt="Elbow_Plot png" src="https://github.com/user-attachments/assets/3812a2ab-3ae3-4d69-a1d6-af4b4993a9d3" />
                                      
Cluster_plot.png
<img width="889" height="442" alt="Cluster_Plot png" src="https://github.com/user-attachments/assets/95b5dadf-6283-45f5-b211-c18e9388c698" />
                                            


📈 Visual Outputs
Elbow Method	Cluster Boundaries

🏁 Conclusion

This short yet impactful project demonstrates how unsupervised learning (K-Means) can uncover patterns in keyword performance.
The clustering approach helps marketers or analysts quickly identify groups of keywords with similar behavior and cost patterns — paving the way for smarter decision-making.

You can view and run this project directly in Google Colab here:  
👉 [Open in Google Colab](https://colab.research.google.com/drive/12tTtzxka9_m9Vy7ounsnC6Rhkvx7QyCK?usp=sharing)

👩‍💻 Author

Huda Shaikh
Certified Data Analyst | Passionate about turning data into stories
📧 (mailto:hudashaikh.gp@gmail.com)
📍 Pune, India

⭐ If you liked this project, don’t forget to star this repo and connect with me for collaboration opportunities!
