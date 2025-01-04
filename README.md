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
| **Metric**                    | **Spectral Clustering** | **K-Means Clustering** |
| ------------------------------ | ----------------------- | ---------------------- |
| Optimal Clusters (k)           | 8                      | 2                     |
| Silhouette Score               | 0.372                  | 0.483                 |
| Key Teams in Top Cluster       | Liverpool, Man City    | Chelsea, Liverpool, Man City |
| Cluster Characteristics        | Granular Clustering    | Clear Performance Separation |
| Teams per Cluster              | 11 (Top Cluster)       | 3 (Top Cluster)       |

📌 **Key Insight:** K-Means clustering provided clearer team segmentation based on performance, while Graph-Based clustering captured more subtle performance differences across teams.

---

## 📊 Visualizations
- **PCA Visualization:** Displayed team clusters in a reduced 2D space.
- **Cluster Heatmaps:** Compared key metrics (goals, points, fouls) across clusters for both methods.

---

## 📦 Repository Structure
├── data/ # Raw and processed datasets ├── notebooks/ # Jupyter notebooks for data preparation and clustering analysis ├── visuals/ # Visualizations generated (PCA, Heatmaps) ├── src/ # Python scripts for data preprocessing and clustering ├── reports/ # Final analysis report and findings ├── README.md # Project description and summary

yaml
Copy code
