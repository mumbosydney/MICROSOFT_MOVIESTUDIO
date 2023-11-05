Microsoft Movie Analysis
##Author: Sydney Mumbo

#Overview
Microsoft have decided to create a new movie studio and require more insight into which types of films are doing best at the box office. This project uses descriptive statistical analysis on data gathered from IMDb website to gain insight into which combination of genres topped the box office in these areas. Three seperate datasets were used for this analysis to gain insight into which combination genres of movies had the top average ratings and number of votes. The results of the top 10 combination genres in averating rating is Comedy,Documentary and Fantasy and number of votes was clearly the combination Action, Fantasy & War, with adventure being present in the majority of the top 10 of the 2 categories. My recommendation for which type of Movie to produce would be Action, Fantasy & War as this is the most predominant combination in the analysis. Drama was also clearly a strong genre for popular successful movies and I would recommend other genres being paired with  Drama during production.

#Business Problem
Microsoft sees all the big companies creating original video content and they want to get in on the fun. They have decided to create a new movie studio, but they don’t know anything about creating movies. You are charged with exploring what types of films are currently doing the best at the box office. You must then translate those findings into actionable insights that the head of Microsoft's new movie studio can use to help decide what type of films to create.
Data
The data analysed came from IMDb website. IMDb (an acronym for Internet Movie Database) is a popular worldwide online database of infomation relating to all movies, television programs, video games and streaming content online. I used 3 files from IMDb to answer the question of which genres were most successful, mainly focusing on the average ratings given and number of votes received.
After checking the information on each table to see column names and null values, I joined the two datasets, titles_basics and title_ratings together using the 'tconst' column as it was a unique identifier creating a new dataframe called df3. I then cleaned up the data by removing null values.
On the bom.movie_gross,I tidied up the "Domestic Gross' and 'Foreign Gross' columns and converted foreign_gross to float datatype to achieve mathematical functons on it. 

#Methods
The data analysed came from IMDb website. IMDb (an acronym for Internet Movie Database) is a popular worldwide online database of infomation relating to all movies, television programs, video games and streaming content online. I used 3 files from IMDb to answer the question of which genres were most successful, mainly focusing on the Domestic and Foreign Gross sales along with average ratings given and number of votes received and equally the runtime of the movies.
After checking the information on each table to see column names and null values, I joined the two datasets, df_titles_basic_info and df_ratings together using the 'tconst' column as it was a unique identifier creating a new dataframe called df3.I cleaned up the null values by removing them and deleted the primary title column.
I used the bom.movie.gross file on its on to carry out the analysis.I created a column for the total gross by calculating the sum of the foreign gross and domestic gross.This new column was used in calculating the average total gross of each studio house to determine which production house has more gross income.

#Results
2 of the above graphs, Top 10 genres by average rating and top 10 genres by Number of Votes clearly show that Adventure, Fantasy and War combination are most successful by number of votes and Comedy,Documentary and Fantasy are popular in terms of average rating. 

The 1st graph showing Genre Distribution shows Drama as top as a solo genre.

To improve confidence in the results next time I would:-

Include movie classification data, such as content advisories (e.g., violence, language, etc.). This additional information can help in narrowing down the target audience for the most successful movies. It will provide insights into which movie classifications are more likely to perform well at the box office.
Perform a temporal analysis by breaking the data into relevant years. This will enable you to track changes in the top genres of movies over time and identify evolving audience tastes. 

#Conclusions
This analysis leads to three recommendations that could could be used by Microsoft in the launching of its movie studios: 
Microsoft should seek to release movies with runtimes of 60 minutes and below since they tend to have higher average ratings.They should aim for movie runtimes within this range to maximize audience satisfaction.Most movies released are of the Drama genre and due to its requent production,Microsoft can look into incorporating drama into its movies since most releases are within that genre.HC being the studio with the highest average gross,Microsoft should seek to partner with HC studio for its movies production due to its high rating gross income.

#Repository Structure

├── MICROSOFTREADME.md                           <- The top-level README for reviewers of this project
├── MICROSOFT MOVIE STUDIO.ipynb   <- Narrative documentation of analysis in Jupyter notebook
├── MicrosoftPresentation.pdf         <- PDF version of project presentation
