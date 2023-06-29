# TubeInsights - Yes Theory YouTube Channel
The project aims to analyze the performance and trends of a YouTube channel using data obtained from the YouTube Data API. By leveraging the API, the project fetches valuable insights about a specific channel, such as its subscriber count, total views, number of videos, and related statistics. Additionally, it explores the video details, including view counts, likes, comments, and durations, allowing for a deeper understanding of video performance.

![image](https://github.com/prajjwalyd/TubeInsights/assets/111794524/e55ed366-5322-4ca2-8fce-bee1c9f8a3af)


The project begins by retrieving channel statistics, including subscriber count, total views, and number of videos. It then fetches the upload playlist ID, which is used to obtain video IDs associated with the channel. Further, it retrieves detailed information about each video, such as its title, description, tags, publication date, duration, and various engagement metrics.

Once the data is collected, the project engages in data manipulation and analysis. It includes data cleaning steps to handle missing values and convert relevant columns to numeric types. The analysis explores various aspects of the video data, including distributions of views, likes, and comments, as well as identifying the top videos with the most views, likes, and comments.

The project also delves into natural language processing techniques, such as generating word clouds to visualize common words in video titles, descriptions, and tags. This provides insights into the content and themes of the videos. Additionally, the project examines the upload schedule by analyzing the publishing day trends, helping understand the channel's consistency.

To gain further insights, the project investigates correlations among video metrics, such as views, likes, and comments, using correlation matrices, pair plots, and box plots. This analysis aids in understanding the relationship between engagement metrics and identifying any patterns or trends.

It seems that you have provided a Python code that uses the YouTube Data API to retrieve data about a YouTube channel and its videos. The code performs various tasks such as fetching channel statistics, retrieving video details, and conducting exploratory data analysis.

![image](https://github.com/prajjwalyd/TubeInsights/assets/111794524/d3503310-5c88-419c-9090-5dadf8f9bb61)

### Here is a breakdown of the code:👩‍💻

1. The necessary libraries and modules are imported, including `googleapiclient.discovery` for accessing the YouTube API, `pandas` for data manipulation, `seaborn` and `matplotlib` for data visualization, and `nltk` for natural language processing tasks.

2. The API key is assigned to a variable `api_key`.

3. The `channel_ids` variable is set to a list containing the channel ID(s) for which you want to retrieve statistics.

4. The YouTube API service name and version are specified, and an API client is created using the `build` function.

5. The `get_channel_stats` function is defined to retrieve channel statistics for the given channel ID(s). It makes use of the YouTube API's `channels().list` method to request the desired statistics.

6. The `get_video_ids` function is defined to retrieve video IDs from a playlist. It uses the YouTube API's `playlistItems().list` method to request the playlist items and extract the video IDs.

![image](https://github.com/prajjwalyd/TubeInsights/assets/111794524/be9f8c90-1c9c-48cc-8678-12acda5fe5dd)

7. The `get_video_details` function is defined to retrieve details of videos. It uses the YouTube API's `videos().list` method to request the video details, including snippet, contentDetails, and statistics.

8. The `get_channel_stats` function is called with the `youtube` and `channel_ids` variables to retrieve channel statistics. The result is stored in the `channel_stats` DataFrame.

9. The `playlist_id` is obtained from the channel statistics.

10. The `get_video_ids` function is called with the `youtube` and `playlist_id` variables to retrieve video IDs. The result is stored in the `video_ids` list.

11. The `get_video_details` function is called with the `youtube` and `video_ids` variables to retrieve video details. The result is stored in the `video_df` DataFrame.

12. Data manipulation and analysis tasks are performed on the `video_df` DataFrame, including handling null values, converting data types, extracting additional information from columns, and calculating derived columns.

13. Exploratory data analysis (EDA) is conducted using various visualizations, such as histograms, bar plots, word clouds, correlation matrix, pair plot, and boxplot. The EDA explores the distribution of views, likes, and comments, identifies top videos with the most views, likes, and comments, visualizes word clouds for video titles, descriptions, and tags, examines the upload schedule, and analyzes the correlations between view count, like count, and comment count.

### Skills:
Python Programming, API Integration, Natural Language Processing (NLP), Sentiment Analysis, pandas, matplotlib, seaborn, Data Manipulation, Data Analysis, Data Visualization, 
