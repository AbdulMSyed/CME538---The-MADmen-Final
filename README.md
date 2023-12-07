# CME538---The-MADmen-Final
YouTube Sentiment Analysis Readme File

Overview
This Python script performs sentiment analysis on YouTube comments related to Formula 1 drivers. It utilizes the YouTube API to gather comments and FastF1 to retrieve information about Formula 1 races. The sentiment analysis is based on a predefined lexicon of words with associated polarities.

Prerequisites
Before running the script, ensure that you have the required libraries installed. You can install them using the following:

pip install google-api-python-client pandas seaborn matplotlib fastf1
Additionally, you need a Google Cloud API key, as indicated in the script, details about aquiring this key can be found in the Medium article.

Code Structure
Setup and Imports:
Import necessary libraries, including the YouTube API, FastF1, and sentiment analysis tools.

Configure Notebook:
Configure the Jupyter Notebook settings, such as plotting styles and suppressing warnings.

YouTube API Configuration:
Set up the YouTube API with the required service name, version, and developer key.

Comment Retrieval Function:
Define a function (get_comments) to retrieve comments for a given YouTube video ID. Handles pagination to get all comments.

Video Retrieval Function:
Define a function (get_videos) to retrieve video IDs from a YouTube playlist.

Sentiment Analysis Function:
Define a sentiment analysis function (sentiment) that calculates sentiment scores for comments related to specific drivers within a given date range.

Lexicon Initialization:
Load a lexicon of words with associated polarities from the 'vader_lexicon.txt' file.

Driver Names:
Define lists of driver names for sentiment analysis.

Sentiment Analysis and Plotting:
Perform sentiment analysis for selected drivers within specific date ranges and plot the results using matplotlib.


Usage
Obtain a Google Cloud API key and replace the placeholder dev_key in the script with your actual key.

Run the script in a Jupyter Notebook.

Customize the script as needed, adjusting driver names, date ranges, and any other parameters.

Execute the cells to retrieve comments, perform sentiment analysis, and generate plots.

Important Note
The script performs sentiment analysis based on a predefined lexicon, and the accuracy of sentiment scores depends on the lexicon's coverage of Formula 1-related terms.
Ensure compliance with YouTube API usage policies and quotas to avoid any disruptions in data retrieval.
Adjust date ranges, driver names, and other parameters as needed for specific analyses.

Author
This script was created by The MADmen. Feel free to contact us for any questions or suggestions.

Refer to the accompanying Medium article for additional insights and guidance on using the script.
