# CME538---The-MADmen-Final
YouTube Sentiment Analysis

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

---------------------------------------------------------------------------------------------------------------------------------------------------------
Formula 1 Telemetry Analysis

This repository contains Python code for analyzing Formula 1 telemetry data using the FastF1 library. The code explores various aspects such as driver performance, braking points, and final race positions over multiple years.

## Prerequisites
Ensure you have the following libraries installed:
- os
- numpy
- pandas
- seaborn
- matplotlib
- fastf1

## Getting Started
1. Import necessary libraries.
2. Configure the notebook with matplotlib settings and suppress warnings.
3. Explore telemetry data to understand its structure.

## Analysis Sections
### Section 1: Throttle Comparison (Qualifying)
- Retrieve telemetry data for Charles Leclerc and Max Verstappen during the 2023 Mexico Grand Prix Qualifying session.
- Compare their throttle usage during the first 30 seconds of the session.

### Section 2: Brake Points Comparison (Qualifying vs Race)
#### Subsection 2.1: Sergio Perez
- Compare braking points for Sergio Perez during the 2023 Mexico Grand Prix Qualifying session and a practice lap.
#### Subsection 2.2: Perez vs Leclerc
- Compare braking points for Sergio Perez and Charles Leclerc during lap 1 of the 2023 Mexico Grand Prix.
#### Subsection 2.3: Brake Points and Track Overlay (First Turn)
- Overlay braking points and track positions for Perez and Leclerc during the first turn of lap 1 with an offset.

### Section 3: Brake vs Position (Race)
- Compare brake usage and positions on track for Sergio Perez and Charles Leclerc during lap 1 of the 2023 Mexico Grand Prix.

### Section 4: Final Positions Analysis (2017-2021)
- Analyze final race positions for Lewis Hamilton and Valtteri Bottas from 2017 to 2021.

### Section 5: Additional Analysis (Gasly and Albon - 2019-2020)
- Analyze final race positions for Pierre Gasly and Alexander Albon during 2019 and 2020.

## Conclusion
This code provides insights into Formula 1 telemetry data, allowing for a detailed analysis of driver performance, braking points, and final race positions.

Feel free to explore and adapt the code for your specific analysis needs.
