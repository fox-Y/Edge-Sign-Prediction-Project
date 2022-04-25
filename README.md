# Edge-Sign-Prediction-Project
In our project, we would first deal with the graph data and obtain an undirected graph. Following this, we would do testing and decide on the model we would use. Then, we can use machine learning to predict the formation of links between the unconnected node pairs of the graph. After conducting the link formation, we would further predict the characteristic of these links in terms of positive or negative.

# Dataset
## Bitcoin OTC trust weighted signed network
This is who-trusts-whom network of people who trade using Bitcoin on a platform called Bitcoin OTC. Since Bitcoin users are anonymous, there is a need to maintain a record of users' reputation to prevent transactions with fraudulent and risky users. Members of Bitcoin OTC rate other members in a scale of -10 (total distrust) to +10 (total trust) in steps of 1. This is the first explicit weighted signed directed network available for research.
## Data format
SOURCE: node id of source, i.e., rater/n
TARGET: node id of target, i.e., ratee
RATING: the source's rating for the target, ranging from -10 to +10 in steps of 1
TIME: the time of the rating, measured as seconds since Epoch. 
