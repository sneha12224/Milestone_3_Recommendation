# Milestone 3: Recommendation Engine  
## StudyTrack_AI_StudentRecommend  


##  Objective
The goal of this milestone is to build a **Recommendation Engine** based on the **ClusterID** generated in Milestone 2.  
Each cluster represents a group of students with similar study behaviors and performance patterns.  
The engine provides **personalized recommendations** to help students improve their academic performance.

---

##  Dataset Source
- Dataset used: `clustered_students.csv` (generated in Milestone 2)
- Location: `/StudyTrack_AI_StudentRecommend/Milestone_2_Clustering/`
- Source: Derived from student study performance dataset used in Milestone 1 & 2  
- Includes columns such as:  
  `study_hours`, `performance_score`, and `ClusterID`

---

##  Steps Followed
### 1. **Cluster Mapping**
- Loaded the clustered dataset from Milestone 2.
- Verified the presence of the `ClusterID` column.
- Analyzed characteristics of each cluster (high, medium, and low performers).

### 2. **Recommendation Generation**
- Created a Python function `generate_recommendation(cluster_id)` to map each cluster to a meaningful recommendation.
- Added a new column `Recommendation` to the dataset.
- Example mapping:
  - **Cluster 0:** High performers → “Maintain consistent study routine.”
  - **Cluster 1:** Medium performers → “Increase study hours by 1 hour/day.”
  - **Cluster 2:** Low performers → “Focus on basics and seek mentorship.”

### 3. **Visualization**
- Created a **count plot** showing the number of students per recommendation type.

##  Tools Used
- **Google Colab** – Code execution and visualization  
- **Python Libraries:**
  - `pandas` – Data loading and manipulation
  - `matplotlib`, `seaborn` – Visualization
  - `os` – File handling

##  Key Insights
- Clustering helped to identify 3 main student performance groups.
- Recommendations are data-driven, ensuring targeted improvement strategies.
- Visualization clearly shows which type of students dominate (e.g., majority medium performers).


##  Conclusion
This milestone successfully developed a **Recommendation Engine** that converts clustering insights into **personalized study improvement plans**.  
These recommendations will serve as the foundation for an AI-based student support system in the next stage of the project.
