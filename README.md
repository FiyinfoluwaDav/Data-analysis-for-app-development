# Data Analysis for Profitable App Profiles

## Overview

This project focuses on analyzing mobile app data to identify profitable app profiles for both the App Store and Google Play markets. The goal is to provide data-driven insights for developers on what kinds of apps are most likely to attract users and generate revenue through in-app advertisements.

## Project Objective

The primary aim is to analyze data from the App Store and Google Play to understand which app categories and genres are the most successful in terms of user engagement. Since the focus is on free-to-download apps that generate revenue via in-app ads, the number of users is the key metric for profitability.

## Data Sources

The analysis is based on two datasets:

-   **Google Play Store Apps:** A dataset of over 10,000 apps from the Google Play Store. [Link to the dataset on Kaggle](https://www.kaggle.com/datasets/lava18/google-play-store-apps)
-   **App Store Apps:** A dataset of over 7,000 apps from the Apple App Store. [Link to the dataset on Kaggle](https://www.kaggle.com/datasets/ramamet4/app-store-apple-data-set-10k-apps)

The data is located in the `csv files` directory.

## Methodology

The analysis was conducted in the `Data_analysis_for_app_profiles.ipynb` Jupyter Notebook and involved the following steps:

### 1. Data Cleaning and Preprocessing

-   **Handling Incorrect Data:** A row with inconsistent data in the Google Play dataset was removed.
-   **Removing Duplicates:** Duplicate app entries were removed from the Google Play dataset. The entry with the highest number of reviews was kept, assuming it to be the most recent.
-   **Filtering by Language:** Both datasets were filtered to include only apps with English-language names.
-   **Filtering by Price:** The analysis is focused on free apps, so all paid apps were removed from both datasets.

### 2. Exploratory Data Analysis

-   **Frequency Analysis:** The frequency of apps in each category (Google Play) and genre (App Store) was calculated to identify the most common app types.
-   **Popularity Analysis:**
    -   For the App Store, the average number of user ratings for each app genre was calculated as a proxy for popularity.
    -   For the Google Play Store, the average number of installs for each app category was calculated to determine popularity.

## Key Findings

-   **App Store:** The analysis of user ratings suggests that **Social Networking** and **Music** apps are among the most popular genres. However, the market is dominated by a few major players. A more niche area with high user engagement could be a good target.
-   **Google Play:** The analysis of installs indicates that categories like **Communication**, **Social**, and **Video Players** have a very high number of users. The **Art & Design** category also shows a significant number of installs, suggesting a potentially profitable niche.

Based on the analysis, developing an app in a popular category that is not overly saturated could be a good strategy. For example, a niche social networking app or a creative app in the "Art & Design" category could be a profitable venture.

## Project Structure

```
.
├── Data_analysis_for_app_profiles.ipynb  # Jupyter Notebook with the data analysis
├── README.md                             # This README file
└── csv files/
    ├── AppleStore.csv                    # App Store dataset
    └── googleplaystore.csv               # Google Play Store dataset
```

## How to Run the Analysis

1.  Clone the repository.
2.  Make sure you have Jupyter Notebook installed.
3.  Open and run the `Data_analysis_for_app_profiles.ipynb` notebook.

## Author

-   **Fiyinfoluwa David** - [FiyinfoluwaDav](https://github.com/FiyinfoluwaDav)