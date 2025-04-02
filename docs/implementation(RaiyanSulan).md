# Implementation (Everything done by Raiyan Sultan)

## Introduction
The dataset utilized for this project is the Air Quality Dashboard Map from Bristol Open Data, (https://opendata.bristol.gov.uk/maps/a26113cd0bef4ef0816242a08ae0b1a6/explore). It provides annual NO₂ (nitrogen dioxide) concentration levels for selected areas within Bristol. Additionally, it includes historical NO₂ data, allowing users to analyze past air quality trends in these regions.

One of the key features of this dataset is its interactive search functionality, which enables users to locate and view NO₂ concentration data for specific locations marked on the map. However, a known limitation is that it does not provide air quality information for unmarked areas, meaning that some locations may not have recorded data available.

As of the most recent update, the dataset was last recorded on December 13, 2024.

## Project Structure
done with the help of ChatGPT
[code2.zip](https://github.com/user-attachments/files/19555983/code2.zip)

![image](https://github.com/user-attachments/assets/caca03f6-85a6-47fd-9c9f-87cc05d0ca1a)


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
Example of the UML which was already provided.

![UML Class diagrams representing JSON query results](images/class1.png)


Used the help of ChatGPT to make A simple UML for AirAware

![image](https://github.com/user-attachments/assets/4f5673a8-de06-4801-a0b1-68a49c5bc056)


# User guide

## USER CASE 1 : View Air Quality of a Location

1. Run home.html, which will then redirect you to the website through your default browser
![image](https://github.com/user-attachments/assets/f569bb72-37a4-4c37-a6e4-f5ab6d5b2843)

2.User Selects the button "View AQI MAP" to enter the maps section.
![image](https://github.com/user-attachments/assets/f08b7f22-f542-4b4d-b3a5-3016d3b11e8c)

3. On first use, the users will be given a cookies option, the user should put whichever option they prefer.

![image](https://github.com/user-attachments/assets/11e0fd5b-584c-4d2e-be07-18a3b908f92b)

4. The user will have 2 options to check the air quality of their desired area.

![image](https://github.com/user-attachments/assets/39757b9e-8480-4f7b-8997-7232e3845505)

4 A. Option 1- clicking on a marker and checking the air quality, NO2 levels.

It will show the annual NO2 at first.

![image](https://github.com/user-attachments/assets/93a5b196-f3ae-4a14-9ca6-d586b08e4993)

here they can check the annual NO2 levels for the area, by clicking on the button on the bottom right, from 2010-2023.

![image](https://github.com/user-attachments/assets/9c428db0-2243-4c30-904f-d519babbf382)


but scrolling the small box lower will reveal the historical annual levels of NO2.

![image](https://github.com/user-attachments/assets/baf4d078-84d1-4e90-b43a-9e4bbfb38f35)

4 B. Option 2- clicking Search button and manually putting in their desired area address which will let them see the same things as option 1, but some areas are not covered, so they might not get a search result.

![image](https://github.com/user-attachments/assets/39caad1d-3b53-4abf-b628-40ca351fa4f9)






