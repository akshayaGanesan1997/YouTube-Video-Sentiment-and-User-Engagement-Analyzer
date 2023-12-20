# Youtube Video Sentiment And User Engagement Analyzer

## Overview

This repository contains Python code for analyzing YouTube video data using Google Colab. The analysis includes exploratory data analysis (EDA), sentiment analysis using the RoBERTa model, and user engagement analysis. The dataset used in this project is obtained through the YouTube Data API.

## Prerequisites

Before running the code, you need to set up a Google Cloud project, enable the YouTube Data API, and obtain an API key. Follow the steps below:

1. Go to the [Google Cloud Console](https://console.cloud.google.com/).
2. Click on the project dropdown at the top of the page and click on "New Project."
3. Enter a name for your project and click on the "Create" button.
4. Navigate to "APIs & Services" > "Dashboard." Click on "+ ENABLE APIS AND SERVICES."
5. Search for "YouTube Data API v3" and select it. Click on the "Enable" button.
6. In the left sidebar, click on "Credentials."
7. Click on "+ CREATE CREDENTIALS" and choose "API Key."

   The API key is now created and ready for use. Copy the generated API key and paste it in a text file named 'api_key.txt'. This key will be used in the application to authenticate requests to the "YouTube Data API v3."

## Uploading Code to Google Colab

To run the code in Google Colab, follow these steps:

1. Open Google Colab in your browser: [Google Colab](https://colab.research.google.com/).
2. Open the provided python notebook file (YouTube_Sentiment_Analysis.ipynb) in your Colab environment.

## Uploading Files in Colab

Upload the following files in Colab which is attached with the submission:

1. api_key.txt - Copy the generate API key in previous step here
2. FINAL-YOUTUBE-DATA.csv - YouTube Dataset 
3. YOUTUBE-DATA-Preprocessed.csv - YouTube Dataset with preprocessed data
4. YOUTUBE-DATA-Preprocessed-Sentiments.csv - YouTube Dataset with sentiment labels classified

The following files can be uploaded using the below python code:

```python
from google.colab import files
uploaded = files.upload()
```

## Additional Notes:

Sentiment analysis uses the RoBERTa model, and results are stored in YOUTUBE-DATA-Preprocessed-Sentiments.csv. This takes some time to run since there are a lot of youtube comments to process. Hence, the sentiment classified comments csv file is provided here. Upload it and continue to do user engagement analysis and sentiment analysis on comments.
