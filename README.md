# I310D-Assignment-7-Data-Curation-and-Analysis-MAL
Scraping top 300 anime on My Anime List (MAL) using pandas
Using Python's panda API, I look at data from My Anime List and found the top 300 anime, sorting it by the following categories:
Rank, Anime, Anime type, Episodes, Start air date, End air date, Members, and the Score.
Rank - the rank of the anime, like Bocchi the Rock, at this time, is rank 19.
Anime - the name of the anime
Anime type - some anime are TV shows (they have multiple episodes), some are considered ONO (the chinese anime), some are considered OVAs, some are considered Movies.
Episodes - the number of episodes in the anime
Start air date - the starting air date of the anime in Japan, month and year
End air date - the ending air date of the anime in Japan, month and year
Members - the number of people who have stated they watched the anime on MAL
Score - average rating of an anime by MAL users, this amount of users does not appear in this dataset and is lower than the number of people who have watched a certain anime.


The main goal of this project was for me to find and visualize interesting data based on the website as a fun way to start getting into data curation and analysis.

In the code, two different methods were used to clean the data, although only one is used. I did this in order to learn other, more efficient ways, to clean data.

The data came from these six pages:
https://myanimelist.net/topanime.php?limit=0
https://myanimelist.net/topanime.php?limit=50
https://myanimelist.net/topanime.php?limit=100
https://myanimelist.net/topanime.php?limit=150
https://myanimelist.net/topanime.php?limit=200
https://myanimelist.net/topanime.php?limit=250

After cleaning the data, I created and analyzed a bar chart looking at the number of episodes an anime has and its rank. From this bar chart, one thing that stook out to me was that there are a significant amount of anime movies (the shortest bar which is equivalent to one episode) in the top 300.
However, unsuprisingly, most of the anime in the top 300 are, on average, either 12 or 24 episodes, with some outliers, the anime One Piece having 1049 episodes.

From what I can tell, there are no biases in this data, however, because One Piece is still going on, MAL had its number of episodes as a ?, which led to some troubles. Because of this, and the fact that One Piece is the only case of this, I just coded it to replace the ? with the current number of episodes at this time.

Data.world data: https://data.world/keenanh/i310d-assignment-7-data-curation-and-analysis/workspace/project-summary?agentid=keenanh&datasetid=i310d-assignment-7-data-curation-and-analysis
