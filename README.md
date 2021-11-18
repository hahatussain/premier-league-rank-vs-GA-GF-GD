# Premier League Ranks vs GF/GA/GD

"Attack wins you games, defence wins you titles" is a quote attributed to Sir Alex Ferguson and one that is thrown around a lot. Here, I try to dig into if this is indeed the fact.

![image](https://user-images.githubusercontent.com/78305343/142453181-e0ea0217-038a-48cb-ae10-5218acc3b3aa.png) - credits - u/FL8_JT26 on r/soccer.


If one analyzes this table, it can be concluded that attack is more important to a team's chances of winning the league. Justification : 

1. The team that scored the most goals won 17 of the 28 seasons.

2. The team that conceded the fewest goals won 12 of the 28 seasons.

3. The average league position of the team that scored the most is 1.66.

4. The average league position of the team that conceded the least is 2.1.

Since here we only consider the best attacking and best defending teams per season, the analysis can be prone to bias. So, I tried to consider each team's Goals For and Goals Against. A simple way to go about it was finding relation between both and the team's rank, using linear regression.

# Results : 

Value of R-squared when Goals For is used : 0.6650899983768193

Scatter Plot : 

![image](https://user-images.githubusercontent.com/78305343/142455423-b0dbbc12-af77-460f-adc0-07126891eb1a.png)

Value of R-squared when Goals Against is used : 0.6915940749282808

Scatter Plot : 

![image](https://user-images.githubusercontent.com/78305343/142455620-2a1278f8-8ea4-42fd-9286-aec922448855.png)

This shows that Goals Against is slightly more associated with the rank of a team, thus we can say that having a better defence will give more chances of a better rank.

Albeit all this, 0.69 is still not a convincing number. Upon further analysis, it was found that Goal Difference is much more closely associated with the rank of a team. 

In this case, value of R-squared : 0.8384102509297338 (much better than 0.69)

Scatter Plot : 

![image](https://user-images.githubusercontent.com/78305343/142456615-cb6dc54a-33ed-477b-832e-470ccb64ba8e.png)

Clearly, the plot is much less scattered and the range for each rank is quite less. Thus, although we can't say for sure if defence or attack wins titles, having a good balance between attack and defence will leave a team in a better position to win the league.







