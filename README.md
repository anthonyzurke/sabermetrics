# Baseball Sabermetrics

---

## Table of Contents
1. [Problem Statement](#Problem-Statement)
2. [Preprocessing and Modeling](#Preprocessing-and-Modeling)
3. [Analysis](#Analysis)
4. [Conclusion and Recommendations](#Conclusion-and-Recommendations)
5. [Data Dictionary](#Data-Dictionary)
6. [Datasets](#Datasets)

---

## Problem Statement

In baseball,  a pitcher's success is heavily determined on the outcomes of a batted ball, and a swing and miss. Finding ways to increase success can come in many forms, velocity, spin rate, horizontal, and vertical break all play a key role.

I’ve used advanced sabermetrics from pitcher’s from the past three seasons (2019-2021)  to be able to assess how to use this data to find in-game success. To do this I used an  unsupervised cluster model using KMeans

---

## Preprocessing and Modeling

I used data from Baseball Savant (https://baseballsavant.mlb.com/) from the 2019, 2021 and the shortened 2020 season. All pitchers used had a minimum batters faced of 200 for the 2019 and 2021 data and in the 2020 data minimum of 75 batters faced due to a shortened season, pitch types used were 4 seam fastball, slider, curveball, changeup, and cutter. The variables of interest are all occurrences of batted ball outcomes and metrics such as evit velocity, launch angle, barrel percentage, poor/weak contact, in and out of strikezone swing and swing and miss, expected batting average, expected slugging percentage, expected on base plus slugging percentage. Expected means each batted ball is assigned an xBA based on how often comparable balls, in terms of exit velocity, launch angle and, on certain types of batted balls, Sprint Speed -- have become hits since Statcast was implemented Major League wide in 2015 (https://www.mlb.com/glossary/statcast/expected-batting-average). Imputation included 0 for pitch types that are not in that particular pitcher’s arsenal. 

The model I selected was an unsupervised cluster using K Means. I used Standard Scaler to standardize my data and used pca to narrow down features from 86 to 9. To see the optimal amount of clusters I used the elbow method using inertia and the result I got was 4.

---

## Analysis

|Label          |Cluster 0     |Cluster 1     |Cluster 2  |Cluster 3 |
|---              |---         |---           |---        |---       |
|age              |31.64       |28.8          |29.33      |27.81        |       
|edge%            |42.74       |41.52         |42.68      |43.2          |
|poor_weak%       |4.42        |4.07          |4.67       |4.27          |
|4seam%           |22.34       |37            |0          |43.78          |
|4seam_velo       |92.32       |94.04         |0          |93.18          |
|ch%              |9.4         |5.73          |13.37      |16.63          |
|sl%              |4.82        |33.2          |14.76      |10.72          |
|cb%              |26.4        |0.93          |15.27      |2.62          |
|cu%              |14.95       |4.34          |10.13      |14.64          |
|throws           |0.68        |0.79          |0.53       |0.7          |          

---

## Conclusion and Recommendations

The generalizations I made were to control what you can control. Instead of attacking hitters with their weaknesses, attack with your strengths.
This model can be built upon by adding new features and making more models to see what kind of relationships can be observed.

---

## Data Dictionary

|Feature          |Type     |Dataset                     |Description                       |
|---              |---      |---                         |---                               |
|age              |int64    |mlb_pitch_stats_19_21, 20   |players's age                     |
|edge%            |float64  |mlb_pitch_stats_19_21, 20   |edge of zone percentage           |
|poor_weak%       |float64  |mlb_pitch_stats_19_21, 20   |poor/weak contact percentage      |
|4seam%           |float64  |mlb_pitch_stats_19_21, 20   |4seam fastball percentage thrown  |
|4seam_velo       |float64  |mlb_pitch_stats_19_21, 20   |avgerage 4seam velocity           |
|ch%              |float64  |mlb_pitch_stats_19_21, 20   |changeup percentage thrown        |
|sl%              |float64  |mlb_pitch_stats_19_21, 20   |slider percentage thrown          |
|cb%              |float64  |mlb_pitch_stats_19_21, 20   |curveball percentage thrown       |
|cu%              |float64  |mlb_pitch_stats_19_21, 20   |cutter percentage thrown          |
|throws           |object   |mlb_pitch_stats_19_21, 20   |handedness RHP: 1, LHP: 0         |

---

## Datasets

* [mlb_pitch_stats_19_21.csv]('../datasets/mlb_pitch_stats_19_21.csv'): 2019, 2021 season stats
* [mlb_pitch_stats_20.csv]('../datasets/mlb_pitch_stats_20.csv'): 2020 season stats
* [mlb_pitch_stats_19_20_21.csv]('../datasets/mlb_pitch_stats_19_20_21.csv'): 19, 20, 21 season stats combined
