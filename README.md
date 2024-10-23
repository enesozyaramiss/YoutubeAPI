# YoutubeAPI
![yt-data-api-search](https://github.com/user-attachments/assets/c0960e3a-72c4-4a3f-abf5-9e8661220dba)

## YouTube Shorts Automation Script:
This script automates the process of downloading, processing, and uploading YouTube Shorts videos. It fetches trending English shorts from the USA, processes them by overlaying an image and adding custom audio, generates a random title, description, and tags, and finally uploads the video to YouTube with multi-language support. Additionally, it handles YouTube API authentication and can translate video titles and descriptions into 30 languages.

### Features:
Fetch trending YouTube Shorts from the USA.
Download the most popular short video.
Overlay a custom image and add audio to the video.
Generate random titles, descriptions, and tags.
Add multi-language support for video metadata.
Upload the final video to YouTube.

### Prerequisites:
Before using this script, you'll need to set up the YouTube Data API, generate a token, and install the required dependencies.

### Step 1: Create a Google Cloud Project
Go to the Google Cloud Console.
Create a new project by clicking on the Select a project drop-down at the top, then click New Project.
Name your project (e.g., "YouTube API Project") and click Create.

### Step 2: Enable YouTube Data API
In your project dashboard, go to the Navigation Menu (the three horizontal lines at the top-left corner).
Click on APIs & Services > Library.
In the API Library, search for YouTube Data API v3.
Click on Enable to activate the YouTube Data API for your project.

### Step 3: Create OAuth Credentials
After enabling the API, click on Create Credentials.
Select OAuth 2.0 Client IDs.
Choose Desktop App as the application type and give it a name (e.g., "YouTube API Desktop Client").
After creating the credentials, download the client_secret.json file. This file contains your OAuth 2.0 credentials.
Place this file in the root directory of your project where your Python script will be located.

### Step 4: Install the Required Python Libraries
Use the following command to install the required dependencies:

### !pip install google-auth google-auth-oauthlib google-auth-httplib2 google-api-python-client moviepy googletrans yt-dlp isodate

### This script relies on the following libraries:
google-auth, google-auth-oauthlib, and google-api-python-client: For handling Google OAuth and YouTube Data API requests.
moviepy: For video and audio editing.
googletrans: For translating video titles and descriptions.
yt-dlp: For downloading YouTube videos.
isodate: For handling ISO 8601 formatted durations.

### Step 5: Running the Script
When you first run the script, it will generate a token.pickle file after authenticating your Google account. This file contains your access and refresh tokens for future requests.

