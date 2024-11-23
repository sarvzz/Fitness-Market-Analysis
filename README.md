# Fitness Studio Market Analysis: Exploring Global and National Workout Trends

## Overview

This project analyzes global and national interest in fitness-related keywords using data from Google Trends. It aims to identify peak interest periods, regional preferences, and keyword popularity to support the growth of digital fitness services. The analysis focuses on identifying high-demand areas for virtual home workouts and expanding the studio's offerings effectively.

---

## Key Questions Addressed

1. **Global Trends**:
   - When was the global search for "workout" at its peak?  
     *Saved as*: `year_str`

2. **Keyword Popularity**:
   - Which keyword was most popular during the COVID pandemic?  
     *Saved as*: `peak_covid`
   - What is the most popular keyword now?  
     *Saved as*: `current`

3. **Regional Analysis**:
   - Which country shows the highest interest in workouts: United States, Australia, or Japan?  
     *Saved as*: `top_country`
   - Between the Philippines and Malaysia, which country shows the highest interest in home workouts?  
     *Saved as*: `home_workout_geo`

---

## Data Description

The analysis uses CSV files located in the `Files/data` folder, which include the following:

### 1. **workout.csv**
| Column                | Description                                                                 |
|-----------------------|-----------------------------------------------------------------------------|
| `month`              | Month when the data was measured.                                          |
| `workout_worldwide`  | Index representing the popularity of the keyword 'workout', on a scale of 0 to 100. |

### 2. **three_keywords.csv**
| Column                      | Description                                                                 |
|-----------------------------|-----------------------------------------------------------------------------|
| `month`                    | Month when the data was measured.                                          |
| `home_workout_worldwide`   | Popularity index for 'home workout'.                                       |
| `gym_workout_worldwide`    | Popularity index for 'gym workout'.                                        |
| `home_gym_worldwide`       | Popularity index for 'home gym'.                                           |

### 3. **workout_geo.csv**
| Column                | Description                                                                 |
|-----------------------|-----------------------------------------------------------------------------|
| `country`            | Country where the data was measured.                                       |
| `workout_2018_2023`  | Popularity index for 'workout' during the 5-year period.                    |

### 4. **three_keywords_geo.csv**
| Column                      | Description                                                                 |
|-----------------------------|-----------------------------------------------------------------------------|
| `country`                  | Country where the data was measured.                                       |
| `home_workout_2018_2023`   | Popularity index for 'home workout' during the 5-year period.              |
| `gym_workout_2018_2023`    | Popularity index for 'gym workout' during the 5-year period.               |
| `home_gym_2018_2023`       | Popularity index for 'home gym' during the 5-year period.                  |

---

## Approach

1. **Data Loading and Preparation**:
   - Load CSV files and clean data for analysis.
2. **Trend Analysis**:
   - Identify the peak global search interest for "workout".
   - Compare keyword popularity during the COVID pandemic and the present.
3. **Regional Analysis**:
   - Compare interest levels in workouts across the United States, Australia, and Japan.
   - Analyze home workout interest in the Philippines versus Malaysia.
4. **Insights for Business Expansion**:
   - Identify trends to support the studio's decision-making for virtual workout offerings.

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/sarvzz/fitness-market-analysis.git
   cd fitness-market-analysis
   ```

2. Install dependencies:
   - Required Python libraries:
     ```bash
     pip install pandas matplotlib seaborn
     ```

3. Run the analysis script or Jupyter Notebook:
   ```bash
   jupyter notebook fitness_analysis.ipynb
   ```

---

## Example Insights

- The peak year for global "workout" searches is saved as `year_str`.
- During the COVID pandemic, the most popular keyword was `peak_covid`.
- Currently, the most searched keyword is `current`.
- Among the United States, Australia, and Japan, the country with the highest interest in workouts is `top_country`.
- Between the Philippines and Malaysia, the country with the highest home workout interest is `home_workout_geo`.

---
