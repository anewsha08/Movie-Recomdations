This script demonstrates how to clean, merge, analyze, and visualize movie data using Python and Pandas, focusing on calculating a custom rating metric and displaying the results graphically. 

Brief Explaination of the code:
Data Loading and Preparation:
It loads two CSV files (tmdb_5000_movies.csv and tmdb_5000_credits.csv) using Pandas into movies_df and credits_df.
Renames the movie_id column in credits_df to id for merging.

Data Merging:
Merges movies_df and credits_df on the id column to combine relevant movie data.

Data Cleaning:
Drops unnecessary columns (homepage, production_companies, title_x, title_y).
Drops rows with any missing values.

Calculating Weighted Rating:
Computes a weighted rating for each movie based on vote count (v), average vote (R), a quantile of vote count (m), and mean vote average (C).
Sorts movies by weighted rating in descending order.

Visualization:
Plots a horizontal bar chart showing the top 10 movies based on weighted rating using Matplotlib.
