**SCRAPING YOUTUBE USING YOUTUBE DATA API**

**Project Overview**

This portfolio project focuses on using the YouTube Data API to scrape data from multiple YouTube channels, including channel statistics and video details. The project retrieves channel statistics such as subscribers, views, and total videos, as well as video details such as views, likes, and comments. Additionally, it analyzes and visualizes the collected data.

**Code Description**

The project is implemented in Python and utilizes the googleapiclient library for interacting with the YouTube Data API, pandas for data manipulation, and seaborn for data visualization. Below is a breakdown of the code:

**Importing Libraries**

from googleapiclient.discovery import build

import pandas as pd

import seaborn as sns

**API Key and Channel IDs**

• My API key is AIzaSyB67OdMvQEqeZpW1kthuvMo-r5qVoeEAzo (stored in the api_key variable).

• channel_ids is a list of YouTube channel IDs for which the data was retrieved.

**Channel Statistics Retrieval**

• The get_channel_stats() function retrieves channel statistics for the specified channel IDs, including subscribers, views, and total videos.

• The data is stored in a Pandas DataFrame.

**Data Cleaning**

• The collected data is cleaned by converting numeric columns to the appropriate data types (e.g., subscribers, views, and total videos).

**Data Visualization**

• Data is visualized using bar plots to show the comparison of subscribers, views, and total videos among the selected channels.

• A top 10 list of videos with the highest views is created and visualized in a bar plot.

**Video Details Retrieval**

• The get_video_ids() function retrieves video IDs from a specific playlist (in this case, Ken Jee's uploads).

• The get_video_details() function retrieves video details, including title, published date, views, likes, and comments, for the retrieved video IDs.

**Data Storage**

• The video details data is stored in a Pandas DataFrame and cleaned.

• The data is also aggregated to count the number of videos published per month.

**Data Export**

• The cleaned video details data is exported to a CSV file for further analysis.

**Dependencies**

google-api-python-client

pandas

seaborn


