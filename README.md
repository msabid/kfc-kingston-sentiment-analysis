# KFC-Kingston-Sentiment-Analysis

This repository contains code for extracting and analyzing reviews of KFC locations in Kingston, Ontario using Google Maps API and Google Cloud Natural Language API. Additionally, it includes a Power BI report and a PDF summarizing the customer feedback analysis.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Setup](#setup)
- [Usage](#usage)
- [Data](#data)
- [Reports](#reports)
- [License](#license)

## Introduction
This project aims to gather reviews from KFC locations in Kingston, Ontario, and perform sentiment analysis on the collected reviews. The code extracts reviews using Google Maps API and analyzes the sentiment using Google Cloud Natural Language API.

## Features
- Extracts KFC locations using Google Maps API.
- Collects reviews and place details for each location.
- Performs sentiment analysis on the reviews using Google Cloud Natural Language API.
- Saves the extracted and analyzed data to CSV files.
- Includes a Power BI report summarizing the analysis.

## Requirements
- Python 3.10
- Google Maps API Key
- Google Cloud Natural Language API
- Required Python libraries: `urllib`, `requests`, `pprint`, `pandas`, `google.cloud`
- Power BI Desktop (for viewing/editing the `.pbix` file)

## Setup

### Google Cloud Setup
1. Create a Google Cloud project.
2. Enable the Google Maps API and Google Cloud Natural Language API.
3. Generate an API key for Google Maps API.
4. Set up authentication for Google Cloud services and download the JSON key file.

### Local Setup
1. Clone this repository:
    ```bash
    git clone https://github.com/msabid/kfc-kingston-sentiment-analysis.git
    ```
2. Navigate to the project directory:
    ```bash
    cd kfc-kingston-sentiment-analysis
    ```
3. Install the required Python libraries:
    ```bash
    pip install -r requirements.txt
    ```
4. Set up your environment variables for the Google Maps API key and Google Cloud authentication:
    ```bash
    export GOOGLE_MAPS_API_KEY=your_google_maps_api_key
    export GOOGLE_APPLICATION_CREDENTIALS=/path/to/your/google-cloud-key.json
    ```

## Usage
1. Open the Jupyter Notebook:
    ```bash
    jupyter notebook kfc-kingston-sentiment-analysis.ipynb
    ```
2. Follow the instructions in the notebook to run each cell. The notebook will extract reviews and place details, perform sentiment analysis, and save the data to CSV files in the specified Google Drive folder.

## Data
The repository includes the following CSV files:
- `store_data_reviews.csv`: Contains the extracted review data with sentiment analysis.
- `store_data_place_details.csv`: Contains details of the KFC locations.

## Reports
The repository also includes the following reports:
- `KFC Customer Feedback Analysis, Kingston.pbix`: Power BI report summarizing the customer feedback analysis.
- `KFC Customer Feedback Analysis, Kingston.pdf`: PDF version of the Power BI report.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
