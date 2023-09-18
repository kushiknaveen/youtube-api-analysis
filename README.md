# youtube-api-analysis
How to use Youtube API. Sample Analysis for a Youtube channel

Exploratory Data Analysing Using Youtube Video Data from Most Popular Data Science Channels
1. Aims, objectives and background
1.1. Introduction
Established in 2005, YouTube has evolved into the world's second-largest search engine, processing over 3 billion searches monthly, second only to Google. Despite its prominence, there exists a certain mystique surrounding the inner workings of the YouTube algorithm and the factors influencing a video's visibility and recommendation. YouTube boasts one of the most extensive and intricate recommendation systems in the industrial landscape. For budding content creators, comprehending the criteria behind a video's success can be a formidable task. Numerous misconceptions circulate about what drives a video's popularity, such as the number of likes or comments, or the video's duration. Additionally, it proves beneficial to experiment and identify prevailing trends within specific niches of YouTube content.
Having recently ventured into content creation with a new YouTube channel dedicated to data analytics and data science, I endeavored to glean insights that could prove valuable to fellow novice creators. This endeavor will focus exclusively on data science channels, as other niches may possess distinct characteristics and audience demographics. Thus, this project will delve into the metrics of approximately 10 of the most thriving data science YouTube channels.

1.2. Aims and objectives
Within this project, I would like to explore the following:

Is the quantity of likes and comments influential in garnering more views?
Does video duration impact views and engagement (likes/comments)?
Does title length play a role in views?
What is the typical number of tags for high-performing videos? What are the frequently used tags in these videos?
Examining the upload frequency of creators under consideration and determining which days of the week they tend to upload.
Utilizing NLP techniques to delve into trending topics.
Identifying the prevalent subjects covered in videos (e.g., employing a word cloud for video titles).

1.3. Steps of the project
Obtain video meta data via Youtube API for the top 10-15 channels in the data science niche (this includes several small steps: create a developer key, request data and transform the responses into a usable data format)
Prepocess data and engineer additional features for analysis

## Exploratory data analysis
### Conclusions

1.4. Dataset
Data selection

This project primarily focuses on data science channels, and I discovered that there are limited readily available datasets online that are suitable for this purpose. There were two alternative datasets that I came across:
The top trending YouTube videos dataset on Kaggle: This dataset encompasses several months of data on daily trending YouTube videos across various countries, with up to 200 trending videos per day. However, it wasn't suitable for this project as the trending videos span a wide range of topics unrelated to data science.
Another dataset was sourced from Vishwanath Seshagiri's GitHub repository, containing metadata for over 0.5 million YouTube videos along with their channel data. While there was no explicit documentation on how this dataset was compiled, a cursory examination of the datasets in the repository suggested that the data was gathered through keyword searches for popular terms like "football" or "science." Some relevant keywords like "python" were also included. Despite this, I opted not to utilize these datasets because they lacked data for the channels I was interested in.
I took the initiative to create my own dataset using Google's YouTube Data API version 3.0. The specific steps for data creation are outlined in Section 2: Data Creation below.
Regarding data limitations, although the dataset is applicable for research purposes, it's important to note that my selection of the top 10 YouTube channels for inclusion in the research is based solely on my familiarity with channels in the data science field and may not be entirely accurate. My definition of "popular" is determined solely by subscriber count, yet there are other metrics, such as views and engagement, that could also be considered. Additionally, choosing the top 10 channels may seem somewhat arbitrary given the vast array of channels on YouTube. There may be smaller channels that could also prove interesting to investigate, potentially representing the next phase of this project.

In terms of the ethics of the data source, as per the YouTube API's guidelines, the use of the API is free of charge as long as your application adheres to the specified quota limit for requests. "The YouTube Data API uses a quota to ensure that developers use the service as intended and do not create applications that unfairly reduce service quality or limit access for others." By default, each application is allocated 10,000 units per day, and additional quota can be requested from YouTube API Services if the limit is reached.
Given that all data obtained from the YouTube API is publicly accessible information (visible to everyone on the internet via YouTube), there are no specific privacy concerns from my perspective. Furthermore, the data is acquired solely for research purposes in this case and not for any commercial endeavors.






