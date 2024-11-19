
# Project Name: User Talent Segmentation

This project focuses on analyzing player performance before and after Level 100, clustering users into talent-based segments, and validating the stability of these segments after Level 100. It combines data analysis, clustering algorithms, and statistical verification to provide actionable insights into player behavior.

**You can access data with this link: https://drive.google.com/drive/folders/15-GZ_u7f4SmudzcsTSlGvEFCz68QwtEq?usp=sharing**

## Table of Contents

- [Project Description](#project-description)
- [Technologies Used](#technologies-used)
- [Data Analysis](#data-analysis)
  - [Data Exploration](#data-exploration)
  - [Data Manipulation and Feature Engineering](#data-manipulation-and-feature-engineering)
  - [Data Visualization](#data-visualization)
- [Modeling Approach](#modeling-approach)
  - [Clustering](#clustering)
  - [Segment Validation](#segment-validation)
- [Results and Insights](#results-and-insights)
- [Contact](#contact)

## Project Description

This project segments users based on their performance and behavior before Level 100, using clustering algorithms. It further validates these segments' stability by examining player behavior after Level 100. The results offer insights into player skill levels and spending habits, enabling targeted engagement strategies.

## Technologies Used

- **Python**: Primary programming language.
- **Pandas and NumPy**: For data manipulation and numerical operations.
- **Matplotlib and Seaborn**: For data visualization.
- **Scikit-learn**: For clustering and statistical validation.
- **K-Means Clustering**: For player segmentation.
- **Logistic Regression**: For verifying segment stability.
- **ANOVA Test**: For statistical validation of segment differences.

## Data Analysis

### Data Exploration

- **Dataset Review**: Initial examination of datasets for structure, types, and null values.
- **Player Filtering**: Removed users without data before Level 100 for reliability.
- **Metric Relationships**: Analyzed relationships among metrics like `playon_use`, `level_start`, and `level_end`.

### Data Manipulation and Feature Engineering

- **Feature Creation**:
  - **Win Rate**: Average success rate per player.
  - **Not Completed Count**: Tracks levels exited without completion.
  - **Average Remaining Seconds**: Time left at level completion.
  - **Booster and Playon Use Counts**: Indicates player reliance on support items.
- **Data Merging**: Unified datasets with relevant metrics.
- **Standardization**: Used StandardScaler for better clustering performance.

### Data Visualization

- Visualized success rates, level completion behavior, and booster usage patterns.
- Examined differences in player behavior before and after Level 100.

## Modeling Approach

### Clustering

- **Clustering Algorithms**: Compared three algorithms, selecting K-Means for best divergence.
- **Cluster Validation**:
  - Silhouette Scores: Ensured clustering quality.
  - Elbow Method: Determined optimal number of clusters (N=3).
- **Player Segments**:
  1. **Cluster 0**: Skilled and fast players.
  2. **Cluster 1**: Challenged and disengaged players.
  3. **Cluster 2**: Medium skill and frequent assist users.

### Segment Validation

- **Logistic Regression**: Verified segment stability post-Level 100.
- **ANOVA Test**: Confirmed statistically significant differences among segments.

## Results and Insights

- **Cluster Analysis**: Identified distinct player groups with actionable characteristics.
- **Behavioral Trends**:
  - Skilled players excelled with minimal support.
  - Struggling players required simpler objectives and guidance.
  - Medium-skilled players frequently used support and showed spending potential.
- **Validation**: Segments remained consistent in behavior after Level 100.

## Contact

- **Project Owner**: Çiya Baran Öner
- **Email**: [ciya.baran.oner@gmail.com](mailto:email@example.com)
- **LinkedIn**: [linkedin.com/in/ciyabaranoner](https://linkedin.com/in/ciyabaranoner)
