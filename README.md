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




---

## Preprocessing and Modeling





---

## Analysis






---

## Conclusion and Recommendations




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
