# Edge-Sign-Prediction-Project
In our project, we would first deal with the graph data and obtain an undirected graph. Following this, we would do testing and decide on the model we would use. Then, we can use machine learning to predict the formation of links between the unconnected node pairs of the graph. After conducting the link formation, we would further predict the characteristic of these links in terms of positive or negative.

# Dataset
## Wikipedia Requests for Adminship (with text)
For a Wikipedia editor to become an administrator, a request for adminship (RfA) must be submitted, either by the candidate or by another community member. Subsequently, any Wikipedia member may cast a supporting, neutral, or opposing vote.

We crawled and parsed all votes since the adoption of the RfA process in 2003 through May 2013. The dataset contains 11,381 users (voters and votees) forming 189,004 distinct voter/votee pairs, for a total of 198,275 votes (this is larger than the number of distinct voter/votee pairs because, if the same user ran for election several times, the same voter/votee pair may contribute several votes).

This induces a directed, signed network in which nodes represent Wikipedia members and edges represent votes. In this sense, the present dataset is a more recent version of the Wikipedia adminship election data. However, there is also a rich textual component in RfAs, which was not included in the older version: each vote is typically accompanied by a short comment (median/mean: 19/34 tokens). A typical positive comment reads, "I've no concerns, will make an excellent addition to the admin corps", while an example of a negative comment is, "Little evidence of collaboration with other editors and limited content creation."
## Data format
RES: the outcome of the election (-1 = target was rejected as admin; 1 = target was accepted)  
SRC: user name of source, i.e., voter  
TGT: user name of target, i.e., the user running for election  
VOT: the source's vote on the target (-1 = oppose; 0 = neutral; 1 = support)  
YEA: the year in which the election was started  
DAT: the date and time of this vote  
TXT: the comment written by the source, in wiki markup  
