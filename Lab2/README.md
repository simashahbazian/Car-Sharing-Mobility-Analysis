 🗺️ Car-Sharing & Urban Mobility — Lab 2

📍 **Politecnico di Torino — ICT for Smart Mobility**  
👥 **Group Project — Individual Contribution**

 🎯 Overview

This lab focuses on the analysis of urban mobility patterns in Torino using car-sharing and mobility datasets.

The notebook presents the analytical work contributed individually to **Lab 2, Part 2 through the end of the lab**, covering Origin-Destination (OD) matrix analysis, similarity measurement, and behavioral segmentation.

 🚗 Car-Sharing Rental Validation

The analysis first validates the car-sharing rental records by checking:

- Very short bookings (< 2 minutes)
- Very long bookings (> 24 hours)
- Trips where the vehicle did not move
- Data consistency before OD-matrix analysis

The validation was performed for both **Car2Go and Enjoy** datasets.

 🗺️ Origin-Destination (OD) Matrix Analysis

Car-sharing trips in Torino were mapped to **23 predefined urban zones** and represented as Origin-Destination matrices.

The analysis includes:

- OD matrix construction
- L2 normalization
- OD matrix heatmaps
- Origin and destination spatial patterns
- Comparison of different temporal periods

 Temporal Comparisons

OD matrices were compared across:

- 🗓️ Weekdays vs weekends
- ☀️ Daytime vs nighttime
- 📅 First week vs second week
- 🚗 Car2Go vs Enjoy

These comparisons were used to examine how mobility patterns vary across time periods and between car-sharing platforms.

 📐 OD Matrix Similarity

Four distance metrics were implemented to compare normalized OD matrices:

- **Manhattan Distance (SAD)**
- **Euclidean Distance**
- **Maximum Norm**
- **Spectral Norm**

The analysis included comparisons between different time periods, different weeks, Car2Go vs Enjoy, and random matrices as a reference case.

 Reported Similarity Results

| Comparison | SAD | Euclidean | Maximum Norm | Spectral Norm |
|---|---:|---:|---:|---:|
| Weekdays vs Weekends | 2.507 | 0.201 | 0.100 | 0.129 |
| First Week vs Second Week | 2.512 | 0.163 | 0.038 | 0.056 |
| Car2Go vs Enjoy | 4.594 | 0.349 | 0.176 | 0.222 |
| Random Matrices | 181.075 | 9.511 | 0.963 | 2.670 |

The reported results show the numerical differences between the analyzed OD matrices under the tested scenarios.

 👥 Behavioral Segmentation

The second part of the analysis investigates mobility behavior across different user profiles.

 Gender

OD matrices were generated separately for male and female users and compared using Euclidean distance.

 Age

User mobility patterns were analyzed across age groups using separate OD matrices.

For UnipolTech, the analyzed groups were:

- **Age Group 1:** 11–19
- **Age Group 2:** 20–49
- **Age Group 3:** 50–69
- **Age Group 4:** 70+

 Travel Motivation

Mobility patterns were also compared according to:

- 💼 Work-related trips
- 🏠 Non-work-related trips

The IMQ and UnipolTech datasets were compared using normalized OD matrices and Euclidean distance.

 🔄 IMQ, UnipolTech, Car2Go & Enjoy

The analysis further compares mobility patterns across:

- IMQ
- UnipolTech
- Car2Go
- Enjoy

This includes normalized OD matrices, heatmap visualization, trip-volume comparisons, and behavioral-profile comparisons.

 🛠️ Tools & Methods

- 🐍 Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- GeoPandas
- Shapely
- MongoDB / PyMongo
- OD Matrix Analysis
- L2 Normalization
- Distance Metrics
- Heatmap Visualization
- Behavioral Segmentation

 👤 Individual Contribution

**Group Project — Individual Contribution**

My contribution covers **Lab 2, Part 2 through the end of the lab**, including:

- Car-sharing rental validation
- OD matrix construction and normalization
- Temporal OD analysis
- OD matrix similarity metrics
- IMQ and UnipolTech processing
- Gender-based segmentation
- Age-based segmentation
- Travel-motivation analysis
- Cross-dataset mobility comparisons
- Visualization and interpretation of mobility patterns

 📓 Notebook

The complete portfolio analysis is available in:

`car_sharing_mobility_lab2_portfolio.ipynb`
