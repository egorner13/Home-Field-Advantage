# Home-Field-Advantage
An analysis of the Sporting Phenomena "Home Field Advantage" during the 2021 - 2022 English Premier League Season using SQL and Tableau
## Introduction 
In the English Premier League, 20 teams play 19 games at Home and Away, and collect points based on their performance in a game. A win is worth 3 points, a draw is 
worth 1 point, and a loss is worth 0 points. The goal is to collect as many points as possible throughout the season. At the end of the season, you are placed in a 
position  in the league table equivalent to your total points collected (1st being the highest, 20th being the lowest). Having the most points wins you the league 
trophy. Finishing in the Top 4-7 allows you to compete in Competitions across Europe. However, finish as one of the three lowest point collectors, and you see 
yourself drop down into a lower-level league, where you have to fight to return to the Premier League.

<img width="200" alt="Graph #1" src="https://user-images.githubusercontent.com/73618269/178385216-57a3e6d1-e285-4ecb-9485-adf5f10ed5cc.png">

When teams play, one factor that goes under the radar when discussing team performance and getting as many points as possible is "Home-Field Advantage". This is the 
proposed phenomena that because you are playing on your home field, where your fans are watching you play, you in turn play better and perform at a higher level. 
So, in the context of the recently finished 2021-2022 season, how prominent was "Home-Field Advantage"?

## Was "Home Field Advantage" a real phenomena during the 2021 - 2022 season?
<img width="652" alt="Graph #2" src="https://user-images.githubusercontent.com/73618269/178386146-f57fedaf-a19e-45e9-bfa3-71ce6ab6e615.png">
Above we see a box-and-whisker plot depicting the total goals scored by a teams in the English Premier League both Home and Away. With a higher average, a higher 
25th 
percentile, and a higher 75th percentile, it appears as though teams generally score more goals at Home compared to Away.

<img width="649" alt="Graph #3" src="https://user-images.githubusercontent.com/73618269/178386143-e830934d-df88-49cf-99f9-fe0a5a85560f.png">
Because we've already seen that teams score more goals Home compared to Away, we already know that the average goals allowed Away is greater than at Home. However, 
it's interesting to look at the distribution of data to see how many goals each team allows.

At Home, teams generally allow 15-30 goals total, hence why the box-and-whisker plot appears so condensed. The 4 teams that didn't fall within this range look like 
significant outliers in this data. Away, the total amount of goals allowed is significantly more spread out. However, with a larger IQR and a significantly higher 
75th quartile (25th quartile's being very similar), we can confirm the prior conclusion that generally, more team allow more goals Away than at Home. 

<img width="653" alt="Graph #4" src="https://user-images.githubusercontent.com/73618269/178386895-e9a58fb9-7e3b-4e93-a932-1fd281fe3da8.png">
Through the box-and-whisker plots above, we can see that teams generally performed better at Home compared to Away. The 25th percentile for total points collected 
at Home (22.5) is 6 points better than Away (16.5). The 75th percentile for total points collected at Home (34.5) is 6 points better than Away (28.5). The average 
points collected at Home (28.85) is 5.1 points better than points collected Away (23.75). 

So, generally speaking, teams performed better at Home compared to Away. However, how significant is "Home-Field Advantage" in the context of who's peforming the 
best? Who's finishing the highest in the league?

## Does "Home Field Advantage" and Home vs. Away performance have relevance when determining position in the final standings? 
