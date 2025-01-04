# 📊 Premier League Clustering Analysis (2021-2022)

This project explores clustering techniques to analyze Premier League match data from the 2021-2022 season. Using **Graph-Based Clustering** and **K-Means Clustering**, the goal is to identify patterns and group teams based on their performance metrics. The dataset includes key statistics such as goals scored, fouls committed, and match results, offering a rich foundation for data mining and pattern discovery.

---

## 📈 Project Objective
The aim of this analysis is to:
- Apply **Graph-Based Clustering** and **K-Means Clustering** to Premier League match data.
- Compare the effectiveness of both clustering techniques in grouping teams by performance.
- Use **silhouette scores** and **PCA visualizations** to assess cluster quality and interpret results.
- Gain insights into team similarities, strengths, and weaknesses across the season.

---

## 📊 Dataset Overview
The dataset used in this project consists of:
- **Match-Level Data:** Goals, fouls, yellow/red cards, shots, and match outcomes.
- **Team Rankings Data:** Points, goal difference, and weekly rankings for each team.

📥 *Data Source:* [Kaggle Premier League Match Data](https://www.kaggle.com/datasets/evangower/premier-league-match-data)

---

## 🧑‍💻 Methodology
The project involves the following steps:

### 1. **Data Preparation**
   - Aggregated home and away team statistics.
   - Merged match-level data with team rankings.
   - Selected features for clustering, including performance metrics, discipline metrics, and team rankings.
   - Scaled the features for uniform comparison.

### 2. **Clustering Techniques Applied**
   - **Graph-Based Clustering:** Constructed graphs where nodes represent teams and edges are based on performance similarity.
   - **K-Means Clustering:** Partitioned teams into distinct groups by minimizing variance.

### 3. **Evaluation Metrics**
   - **Silhouette Score:** Used to determine the optimal number of clusters and assess cluster quality.
   - **PCA Visualization:** Plotted 2D projections of clusters for visual interpretation.

---

## 📊 Key Results
| **Metric**                    | **Spectral Clustering**                               | **K-Means Clustering**                   |
| ------------------------------ | --------------------------------------------------- | --------------------------------------- |
| **Optimal Clusters (k)**       | 9                                                   | 2                                       |
| **Silhouette Score**           | 0.372 (moderate cluster separation)                 | 0.483 (better-defined clusters)         |
| **Key Teams (Cluster)**        | - Cluster 0: Diverse mid-performing teams (e.g., Man United, Brighton, Wolves). <br> - Cluster 1: Top performers (Liverpool, Man City). <br> - Clusters 2-8: Individual teams with distinct characteristics (e.g., Chelsea, Arsenal, Norwich). | - Cluster 0: High performers (Chelsea, Liverpool, Man City). <br> - Cluster 1: All other teams (e.g., Man United, West Ham, Everton). |
| **Cluster Characteristics**    | Granular clustering capturing subtle differences between teams. | Simplified segmentation with clear performance distinction. |
| **Teams per Cluster**          | - Cluster 0: 11 teams <br> - Cluster 1: 2 teams <br> - Clusters 2-8: Single teams each | - Cluster 0: 3 teams <br> - Cluster 1: 17 teams |
| **Key Observations**           | More detailed separation with minor performance variations. | Simplified clustering, better suited for high-level segmentation. |


📌 **Key Insight:** K-Means clustering provided clearer team segmentation based on performance, while Graph-Based clustering captured more subtle performance differences across teams.

---

## 📊 Visualizations
The following visuals were used to illustrate the clustering results and provide deeper insights into the differences between Spectral Clustering and K-Means Clustering:

- **PCA Visualization:** A Principal Component Analysis (PCA) plot was used to display team clusters in a reduced 2D space for both Spectral and K-Means clustering. This visual effectively highlights how teams were grouped based on performance metrics. The clear separation observed in K-Means indicates better-defined clusters compared to the more dispersed Spectral clusters.

- **Performance Metrics Bar Plot:** The bar plot compares key performance metrics (Points, Total Goals, and Goal Difference) across clusters. It shows how each cluster differs in terms of average performance, emphasizing how Spectral clustering provides more granular separation, while K-Means offers broader performance distinctions.

- **Discipline Metrics Bar Plot:** This plot visualizes disciplinary metrics (Yellow Cards, Red Cards, and Fouls) across clusters, highlighting the differences in discipline patterns among the clusters identified by both algorithms.

- **Offensive/Defensive Activity Bar Plot:** This plot displays metrics such as Total Shots, Shots on Target, Goals Conceded, and Corners across clusters, providing insights into the offensive and defensive strengths of teams in each cluster.

- **Context Metrics Bar Plot:** The rank distribution across clusters is shown in this visual to illustrate the ranking tendencies within the clusters formed by both methods.

- **Cluster Heatmaps:** Heatmaps were used to summarize the average performance metrics across clusters, including points, total goals, goal difference, fouls, and shots. This visualization makes it easy to compare clusters side by side and observe patterns more effectively.

