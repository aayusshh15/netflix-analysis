# Netflix Titles Analysis

Exploratory data analysis of Netflix movies and TV shows using Python, Pandas, NumPy, and Matplotlib.

## Dataset

Netflix Movies and TV Shows, from Kaggle: https://www.kaggle.com/shivamb/netflix-shows
(about 8,800 titles after cleaning)

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Google Colab

## What I Did

1. **Explored** the data: shape, data types, and missing values
2. **Cleaned** it: filled missing director, cast, and country values with "Unknown", dropped rows with a missing rating or duration, and converted `date_added` to a date to extract the year and month
3. **Analyzed** it with filtering, `groupby`, and `value_counts`
4. **Visualized** it with a bar chart, a line chart, and a histogram

## Summary of Findings

- Roughly 70% of titles are Movies (about 6,100) and 30% are TV Shows (about 2,700).
- The most titles were added in 2019 (about 2,000), after steady growth from 2016. Additions dipped in 2020 and 2021.
- The United States has the most titles (about 2,800), followed by India (about 970), the United Kingdom (about 420), Japan (about 240), and South Korea (about 200).
- Most titles were released in recent years, with a small tail of older titles.

## Caveats

- About 30% of titles had no director and about 830 had no country. I labeled these "Unknown" instead of dropping them.
- Titles with several co-producing countries were counted as separate combinations, so country totals understate how many titles involve each country.
- The 2021 data is likely a partial year, so the drop in additions may be partly due to that.

## Files

- `netflix_analysis.ipynb`: the full notebook with code, charts, and summary
