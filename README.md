# Visualizing_YouTube_Trend

## 1. Introduction
From the start of a video sharing platform, YouTube in 2005, YouTube has been a constantly growing platform and become the world's largest video sharing platform. All the way from cooking courses to courses on how to start learning code, there are tons of video contents that people from all over the world become content creator and also become content user. In this trend, it has become crucial for us, as data scientists, to analyze what contents users watch, whether there are gaps between most watched contents and most produced contents, is there any relationship between number of likes in a single video and number of comments in it, and what are the characteristics of videos that have tons of comments and likes count per views. In this project we will look through, analyze, and visualize YouTube data shared at Kaggle called "Trending YouTube Video Statistics".

## 2. About data set
The dataset has columns</br>
<b>"video_id"</b>: private key of each videos</br>
<b>"trending_date"</b>: date of the video trending</br>
<b>"title"</b>: title of the video</br>
<b>"channel_title"</b>: name of the channel that posted the video</br>
<b>"category_id"</b>: numeric value that shows which category the video is in (Can be matched with categories in YouTube webpage)</br>
<b>"publish_time"</b>: time that the video was published</br>
<b>"tags"</b>: tags that the video has</br>
<b>"views"</b>: number of views</br>
<b>"likes"</b>: number of likes</br>
<b>"dislikes"</b>: number of dislikes</br>
<b>"comment_count"</b>: number of comments</br>
<b>"thumbnail_link"</b>: link to the image of thumbnail</br>
<b>"comment_disabled"</b>: whether writing comment is disabled</br>
<b>"ratings_disabled"</b>: whether the ratings are disabled</br>
<b>"video_error_or_removed"</b>: is there an error with the video</br>
<b>"description"</b>: text discription for the video</br>
Link to the dataset: https://www.kaggle.com/datasnaek/youtube-new

## 3. Key Visualizations
![그림1](https://user-images.githubusercontent.com/56655511/100580590-90be5300-3329-11eb-84a8-e9af72017dc4.png)</br>
This is <b>scatter plot</b> with trend line included with geom_smooth() function. The <b>method</b> was selected to "loess" which is <b>local smooths</b>. We chose this because this method showed most effective on the trend of the data points.</br>
![그림2](https://user-images.githubusercontent.com/56655511/100580854-088c7d80-332a-11eb-947c-de4ec9b5ddf0.png)</br>
This is a <b>normal bar plot</b> with "Whether there is more likes on the video or more dislikes on the video" on x-axis and proportion of having comment disabled on the y-axis.</br>
![그림3](https://user-images.githubusercontent.com/56655511/100581005-4ab5bf00-332a-11eb-9bdd-ca82527089f4.png)</br>
This is a <b>decision tree</b> on how views and comment count allows you to know whether the YouTube video has more dislikes than likes.</br>
We can see that it is difficult to categorize a video whether it has more dislikes than likes with just number of views and number of comments</br>
![그림4](https://user-images.githubusercontent.com/56655511/100581137-8ea8c400-332a-11eb-8069-7c5d051429e4.png)</br>
This is a <b>bar plot</b> with coordinates flipped. The x-axis is title of channels and y-axis is the number of videos that became popular for each channel</br>
![그림5](https://user-images.githubusercontent.com/56655511/100581542-36be8d00-332b-11eb-8fc1-00fe0426a5b5.png)</br>
This is <b>time-series line graph</b>. We can see the trend of total views of YouTube videos in the dataset in trending date</br>
![그림6](https://user-images.githubusercontent.com/56655511/100581700-75544780-332b-11eb-9497-1a05c103e158.png)</br>
This is <b>time-series line graph</b> with trending date as x-axis and count on y-axis. The line graphs are grouped into three sentiment indicators (comments, dislikes, likes)</br>

## 4. Key insights/takeaways about research question
1) We can see that YouTube videos that have <b>more dislikes than likes</b> have about <b>4 times more probability</b> that the video will <b>disable comments</b></br>
2) We <b>cannot predict</b> whether there are more <b>likes than dislikes</b> just by <b>number of comments</b></br>
3) The <b>number of likes</b> went up <b>much faster</b> than number of dislikes or number of comment in YouTube videos</br>
4) The <b>proportion of likes and dislikes</b> have been approximately <b>constant</b> throughout time</br>
5) <b>Music and Entertainment</b> have been <b>most popular YouTube categories</b> in both <b>US and Canada</b></br>
6) <b>Sports and Auto category</b> have been <b>most highlt reacted</b> (by comment) in <b>US</b></br>
7) <b>Movies and Shows category</b> have been <b>most highly reacted</b> (by comment) in <b>Canada</b></br>

## 4. Challenges to be overcomed
1) There were <b>fewer</b> than expected <b>columns</b> of data for us to analyze</br>
: Much more diverse columns would have allowed us to be more creative on analysis</br>
2) <b>Large</b> dataset leading longer loading <b>time</b></br>
: It was quite time consuming to call two large dataset and call other data frame formed from the imported data</br>
3) Could not get <b>optimal decision tree</b></br>
: We could not find how to get optimal decision tree in R</br>

## Reference
Mitchell J. (2019). Trending YouTube Video Statistics.</br>
Retrieved from https://www.kaggle.com/datasnaek/youtube-new</br>
