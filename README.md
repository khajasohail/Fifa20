Business Case :

Explore football skills and cluster football players based on their attributes so that we easly understand who is the best player and with the fifa20 dataset we need to cluster the player by theri skill into certain group.

TASK

Prepare a rank ordered list of top 10 countries with most players. Which countries are producing the most footballers that play at this level?
Plot the distribution of overall rating vs. age of players. Interpret what is the age after which a player stops improving?
Which type of offensive players tends to get paid the most: the striker, the right-winger, or the left-winger?

We have rows - 0 to 18277,Columns - 104 entries,in the fifa20 dataset and we have used KMeans and Hierarchical Clustering and their silhouette score is 0.74 both values are same,and both algorithms are performing well .
DBSCAN gives us silhouette score is 0.79 and we are choosing DBSCAN,for DBSCAN we are using 2 clusters[0,1] by doing Visualization we can say that [0-Every Running PLayers],[1-Goalkeepers]

The analysis of the dataset provided insights into the soccer players' attributes and their relationship with their age and position, 
it also identified the top countries producing footballers and the type of offensive players that get paid the most.
The analysis can help soccer clubs and managers make informed decisions regarding player recruitment and salary negotiations.



RISK


1) The dataset contains 3 different features for player's playing positions detailing their usual positions, club position and the nation position. Of these 3 features, player's usual positions(player_positions) alone can be considered as it does not have any null value. The othe 2 features contain a lot of null values.

2) Several features are not required for the model development like player dob, url etc., This dataset required a huge amount of time in performing the domain analysis to identify the features required for the model development

3) There were missing/null values for few key personal skills(pace, shooting etc.,) which required to be pre-processed before the model development

4) Also, for the positional skills[left striker(ls), center back(cb) etc.,] a) all of the values had incremental ranking of type object(ex: 68+2). Those data were pre-processed into numerical values in the data pre-processing section b) few had missing values which required to be pre-processed for the model development

5) Through a detailed domain analysis, repeatable features provided for the goalkeeping skills were identified and removed before the model development

6) There were null/missing values for few key skills like pace, shooting, dribbling etc., and they we handled during the data pre-processing section
