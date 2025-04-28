# Netflix_DSC_Project

# Netflix Movie Data Analysis Project

## Overview
This project analyzes a dataset of Netflix movies to explore various aspects such as movie genres, popularity, ratings, and release trends. The analysis is performed using Python with libraries like Pandas, NumPy, Matplotlib, and Seaborn for data manipulation and visualization.

## Dataset
The dataset used in this project is named `mymoviedb.csv` and contains the following columns:
- `Release_Date`: The date when the movie was released.
- `Title`: The title of the movie.
- `Overview`: A brief description of the movie (dropped in the analysis).
- `Popularity`: A numerical value representing the movie's popularity.
- `Vote_Count`: The number of votes the movie received.
- `Vote_Average`: The average rating of the movie.
- `Original_Language`: The original language of the movie (dropped in the analysis).
- `Genre`: The genre(s) of the movie.
- `Poster_Url`: URL to the movie's poster (dropped in the analysis).

## Project Steps
1. **Data Loading and Initial Exploration**:
   - Load the dataset using Pandas.
   - Display the first few rows to understand the structure.
   - Check for missing values and duplicates.

2. **Data Cleaning**:
   - Remove unnecessary columns (`Overview`, `Original_Language`, `Poster_Url`).
   - Convert the `Release_Date` column to datetime format and extract the year.
   - Handle missing values and duplicates.

3. **Feature Engineering**:
   - Categorize the `Vote_Average` column into labels like "not popular", "below avg", "average", and "popular".
   - Split the `Genre` column into individual genres and explode the dataframe to have one genre per row for each movie.

4. **Data Visualization**:
   - Create visualizations to explore the most frequent genres.
   - Analyze trends in movie releases over the years.
   - Investigate the relationship between popularity, vote counts, and ratings.

## Key Findings
- **Most Frequent Genre**: Drama is the most common genre in the dataset, followed by Comedy and Thriller.
- **Vote Average Distribution**: Movies are categorized into popularity levels, with a significant portion falling into the "average" and "popular" categories.
- **Release Trends**: The dataset includes movies released over a span of 100 years, with the majority likely concentrated in recent decades.

## Tools and Libraries
- **Python**: Primary programming language.
- **Pandas**: Data manipulation and analysis.
- **NumPy**: Numerical operations.
- **Matplotlib/Seaborn**: Data visualization.
- **Jupyter Notebook**: Interactive environment for code execution and documentation.

## How to Run the Project
1. Clone the repository or download the notebook file.
2. Ensure you have Python and Jupyter Notebook installed.
3. Install the required libraries using `pip install pandas numpy matplotlib seaborn`.
4. Open the notebook and run the cells sequentially to reproduce the analysis.

## Future Work
- Expand the analysis to include more detailed visualizations, such as the distribution of movie ratings over time.
- Incorporate additional datasets to compare Netflix movies with other platforms.
- Build a recommendation system based on genre and popularity.

## Author
Shuvam Chattopadhyay

## License
This project is open-source and available under the [MIT License](LICENSE).
