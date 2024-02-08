## Key passes on half-spaces
Football data analysis on key passes executed on half-spaces. This analysis has been developed based on the Italian Major League SerieA 2021-22 data. I treated this case in my thesis for the course Football Data Analyst provided by [SICS](https://www.sics.it/)

## Goal of the data analysis
This data analysis aims to understand if and how the Serie A men's football teams play over the half spaces by enhancing the concept of *Juego Positional*. In particular, I analyse a particular event data: key passes. Indeed this football event is specific for this game style due to the capacity of breaking a defensive line and playing vertically by reaching or being reached by a team-mate in the half-spaces. Plus, I identified only the *relevant* ones which are key passes that have been propedeutical for a shot or a goal.

## Data Analysis
A first exploratory analysis has been conducted into the dataset to understand which teams produced this type of event data the most, both produced and correctly received (without losing the ball possession).

Furthermore, thanks to the use of heatmaps, I observed in which areas the different teams made more key passes over the season. Hence, by using the **k-means** algorithm, through the **elbow method**, I was able to figure out several clusters for catching where the key passes have been produced. 5 main clusters have been identified. Then, those clusters where the related centroids were close to the half-spaces have been deeply analyzed to understand: the most active players that made this particular football action, who received it the most, and the couple that had a better interaction with. A final table has been developed by catching those Teams that used to search frequently the key passes during the games.

At this point, I developed the metric of key passes weighted. This metric tends to measure and assigns a bonus for all the key passes developed on clusters that represent the half-spaces. The weights have been calculated by the total *relevant* key passes produced divided by the total key passes in each cluster.  $\displaystyle\frac{\sum_{squadre=1}^\text{20} \text{Relevant Key Passes} \text{ * } (1 + w_{cluster=1}^5)}{\sum_{squadre=1}^\text{20} \text{Key passes produced}}$

At this point, I have identified the top 4 SerieA teams that used more to research this type of event data by underlying an attitude or inclination to introduce the *Juego Positional* concept in their game style.

In particular, I proceed to identify the distribution across the pitch of the *relevant key passes* and their distribution broken by clusters. For each team, I also developed a flow map which underlines the zones of intensity and the length of the mentioned *relevant key passes* by exploiting a combination of those produced and received.

## Extra

In order to test how this analysis can be introduced for a focus on the proper team or a Team Opponent Analyst, I focused the attention only on the last 3 games of the season played by A.C Milan.Here, I analyzed the *relevant key passes* produced and received by highlighting the players that made and respectively received the pass and which ones were useful for reaching a goal.

## Libraries

*The following python libraries have been used for this analysis: pandas, numpy, matplotlib, mplsoccer, seaborn and sklearn.* 

## Author
Marco Monini 2023
