# Implementation (Done by Raiyan Sultan)

## Introduction
The dataset utilized for this project is the Air Quality Dashboard Map from Bristol Open Data, (https://opendata.bristol.gov.uk/maps/a26113cd0bef4ef0816242a08ae0b1a6/explore). It provides annual NO₂ (nitrogen dioxide) concentration levels for selected areas within Bristol. Additionally, it includes historical NO₂ data, allowing users to analyze past air quality trends in these regions.

One of the key features of this dataset is its interactive search functionality, which enables users to locate and view NO₂ concentration data for specific locations marked on the map. However, a known limitation is that it does not provide air quality information for unmarked areas, meaning that some locations may not have recorded data available.

As of the most recent update, the dataset was last recorded on December 13, 2024.

## Project Structure
done with the help of ChatGPT
[code2.zip](https://github.com/user-attachments/files/19555983/code2.zip)

![Screenshot 2025-04-01 195055](https://github.com/user-attachments/assets/cf6b373b-3d3c-4dbf-9dca-2965316c24bb)


provide a table listing the number of jslint warnings/reports for each module.

## AirAware Software Architecture
The AirAware software is built using a tree-like structure, meaning users can only move forward or backward between pages in a set path. The main page (home.html) acts as the base, branching out into two other pages: map.html and game.html. (Technically, app.js could be seen as part of game.html since it provides key functions for it.)

1. home.html (Main Page)
This is the starting page of the software. It’s where users first land and can choose to go to either the map or game page.

2. map.html (Air Quality Map Page)
This page lets users view and interact with an Air Quality Index (AQI) map using data from Bristol Open Data. However, it only supports AQI data and does not allow access to any other databases.

3. game.html (Quiz Game Page)
This page features a fun, interactive quiz game where users answer 20 randomly selected questions. It’s designed to be engaging and educational.

4. app.js (Game Functions & Logic)
This script powers the game by handling:

Randomizing questions

Tracking user choices

Giving feedback (like congratulating correct answers)

Storing all the quiz questions

This simple but structured design makes navigation easy while keeping everything organized.

![Screenshot 2025-04-01 194845](https://github.com/user-attachments/assets/dec9c0c4-67db-44fc-8623-d8c59d343c05)

## Bristol Open Data API
TODO: Document each query to Bristol Open Data

![UML Class diagrams representing JSON query results](images/class1.png)
TODO: Repeat as necessary

# User guide
TODO: Explain how each use-case works by providing step-by-step screenshots for each use-case. This should be based on a tested scenario.



