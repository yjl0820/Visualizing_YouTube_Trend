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
This is a scatter ploy with trend line included with geom_smooth() function. The method was selected to "loess" which is local smooths. We chose this because this method showed most effective on the trend of the data points.</br>




## 3. Conclusion

## 4. Challenges to be overcomed
1) There were fewer than expected columns of data for us to analyze</br>
: Much more diverse columns would have allowed us to be more creative on analysis</br>
2) Large dataset leading longer loading time</br>
: It was quite time consuming to call two large dataset and call other data frame formed from the imported data</br>
3) Could not get optimal decision tree</br>
: We could not find how to get optimal decision tree in R</br>

## Reference
