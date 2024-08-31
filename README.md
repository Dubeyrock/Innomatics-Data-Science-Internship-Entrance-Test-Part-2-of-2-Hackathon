# Innomatics-Data-Science-Internship-Entrance-Test-Part-2-of-2-Hackathon
Innomatics Data Science Internship |  Entrance Test (Part 2 of 2) | Hackathon.


Movie Recommendation System
Project Overview
This project involves building a movie recommendation system for Netfiz, a hypothetical streaming platform. The primary objective is to analyze user ratings, movie metadata, and other related data to identify patterns, popular movies, and provide personalized movie recommendations to users. By implementing this system, the platform aims to enhance user engagement and satisfaction, which could lead to increased user retention and revenue.

Dataset Description
The dataset used in this project consists of four CSV files:

movies.csv

Contains movie information, including movie IDs, titles, and genres.
Columns: movieId, title, genres
Shape: (9742, 3)
ratings.csv

Contains user ratings for different movies.
Columns: userId, movieId, rating, timestamp
Shape: (100836, 4)
Unique User IDs: 610
tags.csv

Contains user-submitted tags for movies.
Columns: userId, movieId, tag, timestamp
Shape: Varies depending on the number of tags
links.csv

Contains mapping to external movie IDs, such as IMDB and TMDB.
Columns: movieId, imdbId, tmdbId
Project Workflow
1. Data Exploration and Analysis
Shape and Statistics:

Reviewed the shape of each CSV file to understand the structure of the data.
Extracted basic statistics from the ratings.csv file, including the distribution of ratings, the number of unique users, and movies.
Data Cleaning:

Checked for missing values and handled them appropriately.
Ensured data consistency across different CSV files.
2. Grouping and Aggregation
Grouping Ratings:

Grouped user ratings by movieId.
Applied aggregation functions such as count and mean to calculate the number of ratings and the average rating for each movie.
Filtering Popular Movies:

Filtered the dataset to include only movies that received more than 50 user ratings. This ensured that the recommendations were based on movies with substantial user engagement.
3. Identifying Popular and Highly Rated Movies
Top Movies by Number of Ratings:

Identified the most popular movies based on the number of user ratings. Examples include "Pulp Fiction (1994)", "Shawshank Redemption, The (1994)", and "Matrix, The (1999)".
Top Movies by Average Rating:

Calculated the average rating for each movie and identified movies with high user satisfaction.
4. Web Scraping IMDB Ratings
Scraping IMDB Ratings:

Used the links.csv file to map movies to their IMDB IDs.
Scraped IMDB ratings for movies with more than 50 user ratings to incorporate external data into the analysis.
Identifying Top-Rated Movies:

Identified the movie with the highest IMDB rating and the highest-rated Sci-Fi movie.
5. Conclusion
The project successfully analyzed user ratings and movie metadata, identifying popular movies and calculating average ratings. By filtering for movies with significant user engagement, the project ensured the reliability of the insights generated. The addition of IMDB ratings provided a broader perspective on movie quality.

The final outcome of this project can be used to refine the recommendation algorithms at Netfiz, ultimately improving user engagement by providing personalized movie suggestions that align with user preferences.

Future Work
Expand Data Sources:

Incorporate additional data sources, such as user demographics and watch history, to improve the accuracy of recommendations.
Advanced Recommendation Algorithms:

Implement advanced machine learning techniques such as collaborative filtering, content-based filtering, and hybrid models to enhance the recommendation system.
Real-time Recommendations:

Develop a real-time recommendation engine that updates suggestions based on the user’s current viewing behavior.
Installation and Usage
Requirements

Python 3.11

Pandas
NumPy

BeautifulSoup (for web scraping)

Requests (for web scraping)

Jupyter Notebook (for development and visualization)

Steps to Run the Project

Clone the repository to your local machine.
Ensure all required Python libraries are installed using pip install -r requirements.txt.
Download the dataset and place the CSV files in the appropriate directory.
Run the Jupyter Notebook to execute the data analysis and recommendation pipeline.
License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments
Special thanks to the MovieLens dataset for providing the data used in this project.
Gratitude to the Netfiz team for their guidance and support throughout the project.

