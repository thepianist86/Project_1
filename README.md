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
 
Conclusions: