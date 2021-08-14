# Project_1
Project 1 for NW Data Analysis and Visualization

Scope: Our project is to uncover data trends among all star MLB pitchers from 2015-2019. We will examine relationships between their strikeout %, ERA (earned run average) , BB (walk)%, in their all star seasons, as well as some of their physical dimensions and place of birth (state if domestic, country if foreign born).

Data Cleanup: Roster of all star pitchers was pulled as a CSV file from https://www.baseball-reference.com/ and pitchers stats for 2015-2019 seasons was pulled as a CSV file from https://stathead.com/ . CSV files were imported into dataframes and cleaned and merged using Pandas, then exported to be used in generating various charts. Merged dataframe was then used to query MLB api at http://lookup-service-prod.mlb.com/json/named.search_player_all to generate a dataframe with various player information (e.g. height, weight, birth country, birth state, etc). This dataframe was then cleaned and exported to be used in generating charts.

Charts: Various charts were generated including:
 - ERA+ Boxplot by year
 - All Star vs League Average BB% by year - Bar Chart
 - All Star vs League Average ERA+ by year - Bar Chart
 - All Star vs League Average K% by year - Bar Chart
 - All Star pitchers count by Birth Country - Bar Chart
 - US Born All Star pitchers count by Birth State - Bar Chart
 - All Star pitchers count by height - Bar Chart
 - All Star pitchers count by weight - Bar Chart
 - Scatterplot comparing K% (Strikeouts) and ERA+ for All Star pitchers, with average MLB Pitcher rating graphed for comparison.
 - Scatterplot comparing BB% (Walks) and ERA+ for All Star pitchers, with average MLB pitcher rating graphed for comparison.
 
Conclusions: In terms of statistical data, strikeout percentage is correlated postitively with all star pitchers' performance (using ERA+ as a benchmark). Additionally, the amount of walks (BB%) did not correlate as much with all star pitchers. We conclude that when looking for future all star pitchers, teams should target players with higher strikeout rates, and they are still worth invetsting in even if they walk players. We also determined there is a height threshold of 6 feet 2 inches among all star pitchers where the likeliness they become and all star jumps significantly. We conclude that pitchers who are 6'2 and have a high strikeout rate (usually over 25%) are more likely to become all star pitchers.
