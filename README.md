# CoTrRank_Trust_Evaluation

[![CoTrRank: Trust Evaluation of Users and Tweets](https://i.ytimg.com/vi/eeiMVO4qS1s/hqdefault.jpg?sqp=-oaymwEZCPYBEIoBSFXyq4qpAwsIARUAAIhCGAFwAQ==&rs=AOn4CLCYSz61oHfOt-fc-K1AIciYZ-nKZA)](https://www.youtube.com/watch?v=eeiMVO4qS1s)



# Twitter_Tas_dataset
This is the dataset used for our research project: Trust Evaluation on Twitter. Anyone who are working on data minning, social network analysis, or any related topics can download this dataset for research purposes.

The proposed Co-Rank method and detailed experimental results can be found in our paper: 

## "CoRank A Coupled Dual Networks Approach to Trust Evaluation on Twitter" (WISE 2018).

The data set is designed for research purpose only. There are four files storing the Twitter data crawled from Twitter using its official REST API.

## 'tas_users' 
This file stores all the users in the Tas dataset. We have given each user a user index and the UserID is their original user ID collected from Twitter. These users are crawled based on the 'location' attribute in their profile. They are considered all from the Tasmania Twitter Community.

For Example:

| User_index    | UserID        | 
| ------------- |:-------------:| 
| "7232"        | "1076277643"  | 
| "791"         | "1000773896"  |   

## 'twitter_tweets_all_user_posted'
This file stores all the tweets posted by the users in the Tas dataset. These tweets are crawled from Twitter platform using RestAPI. Please note that, as restricted by Twitter, only a maximum of 3,200 most recent tweets of each user are allowed to be downloaded.

for example: 

| TweetID       | Tweet_index   |  User_index | 
| ------------- |:-------------:| :----------:|
| "100000183710007296"        | "0"  | "12423"|

Because this file is too big, you can download it from [here](https://www.dropbox.com/s/tdxayn1yyy47pi4/twitter_tweets_all_user_posted.txt?dl=0) (*you don't need to create a dropbox account to download the file.*)

## 'twitter_follower_friend_index'
This file stores the follow relations between users. Note that, all the numbers are indicating user_index numbers.

for example: 

| Follower_index| Friend_index  | 
| ------------- |:-------------:| 
| "0"      | "180"  | 

(User_index 0 is following User_index 180)

## 'twitter_tweets_relation_index'
This file stores the retweet and reply relations between tweets. Note that, all numbers are indicating tweet_index numbers.

first column: original_tweet_index | second column: retweet/reply tweet_index | third column: relation type (1 for reply, 2 for retweet)

for example: 

| original_tweet_index| retweet/reply tweet_index  | relation type  |
| ------------- |:-------------:| :----------:|
| "35"      | "40"  | "2" |
| "95"      | "103" | "1" |

Here in relation type, 1 is for reply, 2 is for retweet.
(tweet_index 35 is retweeted by tweet_index 40, and tweet_index 95 is replied by tweet_index 103) 

## 'twitter_user_mention_index'
This file stores the mention relation. User is mentioned by a tweet.

first column: mentioned User_index | second column: tweet_index

for example: 

| mentioned User_index    | tweet_index      | 
| ------------- |:-------------:| 
| "3"        | "1856312"  | 

(user_index 3 is mentioned by tweet_index 1856312)

*Note that, due to the request from Twitter, we can not publish the content of Twitter.*

# References
If you use this data set for research, please cite one of the following papers:

"Peiyao Li,Weiliang Zhao, and Jian Yang. 2018. CoRank: A Coupled Dual Networks Approach to Trust Evaluation on Twitter. In the 19TH International Conference on Web Information Systems Engineering." 
"Peiyao Li,Weiliang Zhao, Jian Yang, and Jia Wu. 2019. CoTrRank: Trust Evaluation of Users and Tweets. In Proceedings of the Twenty-Eighth International Joint Conference on
               Artificial Intelligence, IJCAI-19. PP 6542--6544."

If you have any questions, please do not hesitate to contact me.
