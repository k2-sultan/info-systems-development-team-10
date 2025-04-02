# Implementation (NOTE: EVERYTHING IN THIS FILE WAS CREATED BY ADIELGREAT OLOBAYO)

## Introduction
The name of the Dataset used is Air Quality Dashboard Map (https://opendata.bristol.gov.uk/maps/a26113cd0bef4ef0816242a08ae0b1a6/explore). it contains the annual NO2 in a selected area in bristol and the past NO" concentrations of the area. you can also search using it. of current it was last recorded on the 13th of December 2024. A known issue is the dataset's inability to provide information on all areas apart from if they are marked on the map. 

## Project Structure

Home.html, Map.html, Game.html and app.js was done with the aid of chatgpt

[code2.zip](https://github.com/user-attachments/files/19555983/code2.zip)

![Screenshot 2025-04-01 195055](https://github.com/user-attachments/assets/cf6b373b-3d3c-4dbf-9dca-2965316c24bb)


provide a table listing the number of jslint warnings/reports for each module.

## Software Architecture
Airaware software architecture uses a tree-like architecture where through each branch one can only go back or forward. In this software,e there is only one base page(home.html), and two branch pages(map.html and game.html). (NOTE: you can technically say app.js is a branch of game.html since it borrows its basic functionality from it.)

1. home.html: This serves as the main page(first page) that user interacts with 
    and gives users the option to travel to the other two branch pages.

2. map.html: This serves as a branch page where the user can both view and 
    interact with the AQI map through Bristol Open Data it does not allow the user to view any other type of Database.

3. game.html: This serves as a branch page where the user can interact with the
     system to play a friendly question-and-answer game with the system. Questions are randomized and there are a total of twenty questions.

4. app.js: This is where game.html obtains its functions such as question 
    randomizer, selecting options, congratulation of the user, question selection, etc. This is also where all questions are stored.


![image](https://github.com/user-attachments/assets/548be57a-f2aa-460a-a38f-b4b6a147bbf2)



## Bristol Open Data API
TODO: Document each query to Bristol Open Data

![UML Class diagrams representing JSON query results](images/class1.png)
TODO: Repeat as necessary

# User guide

## USER CASE 1 : View Air Quality of a Location

1.  Run Home.html on a browser
![Screenshot 2025-04-01 201313](https://github.com/user-attachments/assets/6b97f510-47ff-4450-8c92-33de8e54a007)

2.  User selects the button "View AQI MAP"
   
![image](https://github.com/user-attachments/assets/f8248e67-0ea4-48c2-aed7-b9a57e853a28)

![Screenshot 2025-04-01 201356](https://github.com/user-attachments/assets/f9446335-060e-4a00-ab74-fadc62e7569d)

3. User has 2 choices:

     A. Once user is on the map page, user should click on a marker on the map 
        toobtain the air quality of that area on the map.
   ![image](https://github.com/user-attachments/assets/50060627-d81d-49a8-b2e5-96960c06dfe6)

    
     B. Once user is on the map page, user should use the search button on the 
        right side of the map(this method is will not produce a garanteed result as the map only contains
        data on locations indecated on the map).
   ![image](https://github.com/user-attachments/assets/c0e1cd12-8740-4c19-bf48-9b217fb78afa)


## USER CASE 2 : Air Quality Advice Game

1.  Run Home.html on a browser

![Screenshot 2025-04-01 204050](https://github.com/user-attachments/assets/2de1e898-080d-4ac5-8781-d0b9eda08ebe)


2.  User selects the button  "Air Quality quiz"

![image](https://github.com/user-attachments/assets/88ae8b39-d3b6-4bf8-9385-0d273310f474)


3.  Once on the air quality quiz page user will be given to study a question and 
    three optional answers and will be given a choice to which option is the answer to the question(the answer is in the question)

![Screenshot 2025-04-01 204103](https://github.com/user-attachments/assets/16556446-3633-4b0d-8b5c-23be9fde1749)

4. After user selects an answer there are only 2 outcomes;

    A.  User selects the incorrect option, the system will inform the user it is
        incorrect and to try again
   
    ![Screenshot 2025-04-01 204121](https://github.com/user-attachments/assets/5449b5a3-8005-4629-bf88-3d373612f5db)

    B.  User selects the correct option, the system will inform the user it is
        correct and will automatically give user a different question
   
    ![Screenshot 2025-04-01 205219](https://github.com/user-attachments/assets/81c91793-47f9-4cef-ba7a-9c5328e0650a)


6.  If user wishes to obtain another question to try again or does not wish for
    the current question, user can use the button "Reset Game"

![image](https://github.com/user-attachments/assets/7ac7dece-a7fb-4695-80c8-10adf98e2e9e)



