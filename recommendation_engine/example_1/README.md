# Recommendation engine for an online video platform

Today, videos shown to new users on the platform’s home page are manually chosen. You need to implement a recommendation engine to increase the conversation rate.

## Business Questions

1- Classify each video into the following buckets:<br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; o  "Hot" - means trending up. These videos are candidates to be shown. <br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; o  "Stable and Popular" - video view counts are flat, but very high. These videos are candidates to be shown too. <br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; o  "Everything else" - these videos won't be shown. <br>
2- What are the main characteristics of the "hot videos"?<br>
3- After having identified the characteristics of the hot videos, how would you use this information from a product standpoint <br>

## Data Details:

The data provided is in CSV format and in two separate files as summarised below:

File 1: video_count<br>
Columns: <br>
*video_id*: unique video id<br>
*count*: total count of views for the specific video_id on the specific date <br>
*date*: the date that these views occurred<br>


File 2: video_features<br> 
Columns: <br>
*video_id*: video id, unique by video and joinable to the video id in the other table <br>
*video_length*: length of the video in seconds<br>
*video_language*: language of the video, as selected by the user when they uploaded the video <br>
*video_upload_date*: when the video was uploaded<br>
*video_quality*: quality of the video. It can be [ 240p, 360p, 480p, 720p, 1080p] <br>
