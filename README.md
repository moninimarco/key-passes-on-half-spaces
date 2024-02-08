## Key passes on half-spaces
Football data analysis on key passes executed on half-spaces. This analysis has been developed based on the Italian Major League SerieA 2021-22 data. I treated this case in my thesis for the course Football Data Analyst provided by [SICS](https://www.sics.it/)

## Goal of the data analysis
This data analysis aims to understand if and how the Serie A male football teams play over the half spaces by enhancing the concept of *Juego Positional*. In particular, I analyse a particular event data: key passes. Indeed this football event is specific for this game style due to the capacity of breaking a defensive line and playing vertically by reaching or being reached by a team-mate in the half-spaces.

## Data Analysis
A first exploratory analysis has been conducted into the dataset to understand which teams produced this type of event data the most, both produced and correctly received (without losing the ball possession).

Furthermore, thanks to the use of heatmaps, I observed in which areas the different teams made more key passes over the season. Hence, by using the *k-means* algorithm, through the *elbow* method, I was able to figure out several clusters for catching where the key passes have been produced. 5 main clusters have been identified. Then, those clusters where the related centroids were close to the half-spaces have been deeply analyzed to understand: the most active players that made this particular football action, who received it the most, and the couple that had a better interaction with. A final table has been developed by catching those Teams that used to search frequently the key passes during the games.

At this point, I developed the metric of key passes weighted. This metric tends to measure ad assigns a bonus for all the key passes developed on clusters that represent the half-spaces.  
$\displaystyle\frac{\sum_{squadre=1}^\text{20} \text{Key Passes} \text{ * } (1 + w_{cluster=1}^5)}{\sum_{squadre=1}^\text{20} \text{Key passes produced}}$




