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

Above we see a box-and-whisker plot depicting the total goals scored by teams in the English Premier League both Home and Away. With a higher average, a higher 
25th percentile, and a higher 75th percentile, it appears as though teams generally scored more goals at Home compared to Away.

<img width="649" alt="Graph #3" src="https://user-images.githubusercontent.com/73618269/178386143-e830934d-df88-49cf-99f9-fe0a5a85560f.png">

Because we've already seen that teams scored more goals Home compared to Away, we already know that the average goals allowed Away is greater than at Home. However, 
it's interesting to look at the distribution of data to see how many goals each team allowed.

At Home, teams generally allowed 15-30 goals total, hence why the box-and-whisker plot appears so condensed. The 4 teams that didn't fall within this range look 
like significant outliers in this data. Away, the total amount of goals allowed is significantly more spread out. However, with a larger IQR and a significantly 
higher 75th quartile (25th quartile's being very similar), we can confirm the prior conclusion that generally, teams allowed more goals Away than at Home. 

<img width="653" alt="Graph #4" src="https://user-images.githubusercontent.com/73618269/178386895-e9a58fb9-7e3b-4e93-a932-1fd281fe3da8.png">

Through the box-and-whisker plots above, we can see that teams generally performed better at Home compared to Away. The 25th percentile for total points collected 
at Home (22.5) is 6 points better than Away (16.5). The 75th percentile for total points collected at Home (34.5) is 6 points better than Away (28.5). The average 
points collected at Home (28.85) is 5.1 points better than points collected Away (23.75). 

So, generally speaking, teams performed better at Home compared to Away. However, how significant is "Home-Field Advantage" in the context of who's peforming the 
best? Who's finishing the highest in the league?

## Does "Home Field Advantage" and Home vs. Away performance have relevance when determining position in the final standings? 

<img width="653" alt="Graph #5" src="https://user-images.githubusercontent.com/73618269/178389266-126a4ad5-71ad-418a-a99a-7908862ef2af.png">

Notice how 7 of the 8 teams that finished in the highest league positions also had the largest positive difference between Home and Away goals scored (positive 
difference meaning more goals scored at Home than Away). 12 of the 13 teams with a positive goal difference equal to or lower than that of Leicester City (8th place 
finisher) finished below them, and thus below the other 6 teams as well.

The main outlier in this data set is Chelsea. They had the joint lowest positive difference between goals scored at home and away (-4 so they actually scored more 
goals Away than at Home). However, they finished 3rd in the league table. Thus, although we can make a general rule that a larger positive difference in goals 
scored leads to a higher place finish in the league table, it isn't a perfect conclusion.

<img width="531" alt="Graph #6" src="https://user-images.githubusercontent.com/73618269/178389265-e13a4b4f-85d1-47e7-82c5-e34cbe32b571.png">

Here we can see some more insights into Home vs. Away in terms of when you're allowing goals. 9 teams finished with a difference of 6 goals or less between the two 
values (Home and Away). 7 of the teams finished in the top 8 positions of the table, and 2 finished in the last 2 places. Teams with a larger difference in Goals 
Allowed (Home and Away) finished somewhere in the middle of the table. From this data, it appears we can draw the conclusion that the best teams allow fewer goals 
Home and Away, and similarly the worst teams allow a lot of goals both Home and Away.

Manchester United appears to be the only significant outlier data here, finishing in 6th place but allowing 9 more goals Away than at Home. However, it's not nearly 
as big of an outlier as Chelsea previously, as it still only has the 6th highest Goal Allowed Differential amongst the 20 teams. Thus, we can support the conclusion 
drawn above.

<img width="653" alt="Graph #7" src="https://user-images.githubusercontent.com/73618269/178389262-774ba4a2-2912-4cbf-9ff5-f3a53e0e1e19.png">

An incredibly interesting observation can be seen when looking at the 6 teams with the lowest difference in points collected between Home and Away. 3 of these teams 
(Manchester City, Liverpool, Chelsea) finished in the top 3 positions in the league this year. The other 3 (Norwich City, Watford, Burnley)? They were the teams 
that finished in the lowest 3 positions and were relegated into a lower-level league. So, when looking at the total difference between Home and Away, those with the 
lowest difference were at the very extreme's of the spectrum. The best teams perform well Home and Away, and similarly the worst teams perform poorly both Home and 
Away.

Similarly, those teams that aren't as good or bad as these 6 generally find themselves somewhere in the middle of difference in Home vs. Away points collected. The 
teams with the 7th - 10th lowest difference finished anywhere from 12th - 15th place in the table. Of the teams with the 10 highest difference in performance, 8 
finished between 4th -11th. So, based on this data we can see that in most cases, a higher difference in performance lends itself to finishing in a higher position 
that isn't one of the extremes (Top 3 or Bottom 3).  

Tottenham Hotspur represents the most anomolous data to this finding. Despite having the highest difference in Home vs. Away Performance (9 pts more at Home than 
Away), they finished 4th. Everton and Leeds United could also be viewed as anomolous data, as they finished 16th and 17th despite being in the Top 10 in performance 
difference. Thus, although we can make a general rule that a low performance difference leads to either an extremely high or extremely low overall position, and a 
higher difference leads to a position somewhere in the middle of table (with higher performance difference leading to a higher finish relative to the other "middle-
pack teams"), it isn't a perfect conclusion.

### Final General Conclusions
1. "Home Field Advantage" is a phenomena that generally existed in the English Premier League over the 2021 - 2022 Season
    1. Teams generally performed better at Home than Away.
2. Teams that scored significantly more goals at Home than Away finished higher in the standings than their counterparts
3. Teams with the smallest difference in goals allowed at Home and Away finished at polar opposites of the table, either near the top or near the bottom
    1. Good teams had a good defense both Home and Away, and likewise bad teams had a bad defense both Home and Away
4. Teams with the smallest difference in points gained at Home and Away finished at polar opposites of the table, either near the top or near the bottom
    1. Good teams performed well both Home and Away, and likewise bad teams performed poorly both Home and Away

## Disclaimer
For those who have a Tableau license and would like to download my workbook, it can be found above titled "HomeFieldAdvantage.twbx"
