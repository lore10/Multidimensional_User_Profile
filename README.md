Multi-Topic-Preference-Model-for Tweeters -> Datasets-Code

What kind of content are you prone to tweet? datasets used, main code in Python, and results file

Project Abstract

According to tastes, a person could show preference for a given category of content to a greater or lesser extent. However, quantifying people's amount of interest in a certain topic is a challenging task, especially considering the massive digital information they are exposed to. For example, in the context of Twitter, aligned with his/her preferences a user may tweet and retweet more about technology than sports and do not share any music-related content. The problem we address in this paper is the identification of users' implicit topic preferences by analyzing the content categories they tend to post in Twitter. Our proposal is significant given that modeling their multi-topic profile may be useful to find patterns or association between preferences for categories, discover trending topics and cluster similar users to generate better group recommendations of content. In the present work, we propose a method based on the Mixed Gaussian Model to extract the multidimensional preference representation for 399 Ecuadorian tweeters concerning twenty-two different topics (or dimensions) which became known by manually categorizing 68.186 tweets. Our experiment findings indicate that the proposed approach is effective at detecting the topic interests of users.

Multidimensional_User_Profile contains json and ipynb files obtained as a result of the research project . The data corresponds to information analyzed from tweets generated in Ecuador during the month of november 2016. In detail, the files are:

- creators.json 
The creators of tweets per trending topic, the data here is provided for all 1036 trending topics.

- distributors.json 
The distributors who made retweets per trending topic, the data here is provided for all 1036 trending topics.

- unique_users_Creators_Distrib_perTopic368.json
The unique ids of the creators and distributors per trending topic. The data correspond to the 368 trending topics in our project.

- trending_topics_list368.json
The list of the 368 trending topics in our project.

- FollowersCreators_perTrendingTopic (too big, ask to lorena.recalde@upf.edu)
Folder with a list of files with the followers of the creators. A file corresponds to a trending topic creators (and their followers). Those files are used to create the graphs.

- FollowersDistributors_perTrendingTopic (too big, ask to lorena.recalde@upf.edu)
Folder with a list of files with the followers of the distributors. A file corresponds to a trending topic distributors (and their followers). Those files are used to create the graphs.

- Retweeting_graphs368
Folder with the graphs resulting from the application of the RBC method. There are two versions of the graphs per trending topic: json format and gexf format.

- Following_graphs_Creators368
Folder with the graphs resulting after the detection of the "following relationship among creators" per trending topic. There are two versions of the graphs per trending topic: json format and gexf format. Files in the folder FollowersCreators_perTrendingTopic used. These graphs are needed to apply the proposed method TreToc communities.

- Following_graphs_Distributors368
Folder with the graphs resulting after the detection of the "following relationship among distributors" per trending topic. There are two versions of the graphs per trending topic: json format and gexf format. Files in the folder FollowersDistributors_perTrendingTopic used. These graphs are needed to apply the proposed method TreToc communities.

- Our_Method_TretocGraphs368
Folder with the graphs resulting from the application of the TreToc method. The graphs in Retweeting_graphs368, Following_graphs_Creators368, and Following_graphs_Distributors368 were joint. There are two versions of the graphs per trending topic: json format and gexf format.

- Graphs_Extraction.ipynb
Source code implemented to create the graphs for the RBC method and TreToc method.

- Community_Detection_Metrics.ipynb
Source code implemented to calculate the metrics that validate the method proposed. The values for the metrics were calculated over the RBC graphs and TreToc graphs.

- Data_Analysis_Results.numbers
Data that shows the results obtained.

We also provide all the necessary steps to reproduce the experiments on the definition of the Multi-topic preference Model for Tweeters in the paper referenced below. For more details on how these files were generated, we refer to the following 
scientific publication. We would highly appreciate if scientific publications of works partly based on the 
Detection-of-Trending-Topic-Communities_Datasets-Code quote the following publication:

Lorena Recalde and Ricardo Baeza-Yates. 2018. What kind of content are you prone to tweet? Multi-topic Preference Model for Tweeters. In Proceedings of ........., March 26-29, 2018, 14 pages.
