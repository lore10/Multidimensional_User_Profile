Multi-Topic-Preference-Model-for Tweeters -> Datasets-Code

What kind of content are you prone to tweet? datasets used, main code in Python, and results file

Project Abstract

According to tastes, a person could show preference for a given category of content to a greater or lesser extent. However, quantifying people's amount of interest in a certain topic is a challenging task, especially considering the massive digital information they are exposed to. For example, in the context of Twitter, aligned with his/her preferences a user may tweet and retweet more about technology than sports and do not share any music-related content. The problem we address in this paper is the identification of users' implicit topic preferences by analyzing the content categories they tend to post in Twitter. Our proposal is significant given that modeling their multi-topic profile may be useful to find patterns or association between preferences for categories, discover trending topics and cluster similar users to generate better group recommendations of content. In the present work, we propose a method based on the Mixed Gaussian Model to extract the multidimensional preference representation for 399 Ecuadorian tweeters concerning twenty-two different topics (or dimensions) which became known by manually categorizing 68.186 tweets. Our experiment findings indicate that the proposed approach is effective at detecting the topic interests of users.

Multidimensional_User_Profile contains json and ipynb files obtained as a result of the research project . The data corresponds to information analyzed from tweets generated in Ecuador during the month of november 2016. In detail, the files are:

- tweetsNOStemmed_words2vec300.bin (used in 1_ClusteringTweetsKMeans++_Heterogeneity_toPublish.ipynb)
word2vec model for words in vocabulary. Model employed to have the vector representation of the training tweets and experimental users' tweets.

- data_centroids300.json (used in 1_ClusteringTweetsKMeans++_Heterogeneity_toPublish.ipynb)
You will find the vector representation of 22 centroids (however other K values are considered as well). Those were used to initialize EM.

- em_utilities_LORE3.py
Code with EM functions implemented.

- tweetsChosen_vecs1.json (used in 2_UsersModelExample_EM_toPublish.ipynb)
Vector representation (300dim) of tweets (90 citizens + 10 politicians) to run example modeling users with EM.

- responsibility_7Clus_1.json
Soft classification of the tweets in tweetsChosen_vecs1.json after applying EM. (used in 2_UsersModelExample_EM_toPublish.ipynb)

- 1_ClusteringTweetsKMeans++_Heterogeneity_toPublish.ipynb
Code that implements k-means++.

- 2_UsersModelExample_EM_toPublish.ipynb
Example of use of EM algorithm to find the responsibility matrix of tweets (to further model the users).


NOTE: Please, in case of requiring the training tweets contact the autor in lore_10_5@hotmail.com

We also provide all the necessary steps to reproduce the experiments on the definition of the Multi-topic preference Model for Tweeters in the paper referenced below. For more details on how these files were generated, we refer to the following 
scientific publication. We would highly appreciate if scientific publications of works partly based on the 
Detection-of-Trending-Topic-Communities_Datasets-Code quote the following publication:

Lorena Recalde and Ricardo Baeza-Yates. 2018. What kind of content are you prone to tweet? Multi-topic Preference Model for Tweeters. In Proceedings of ........., March 26-29, 2018, 14 pages.
