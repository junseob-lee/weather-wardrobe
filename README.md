Student Name: Junseob Lee

Project Overview: This Android app is designed to help users create suitable outfits based on the day's weather conditions. Users can input their clothing items into a virtual wardrobe, and the app will recommend outfits that are comfortable for the current weather.

Here are the key features of the app: 

Outfit Recommendations: The app generates outfit suggestions based on the daily weather forecast. It ensures that users stay comfortable throughout the day. 
Hourly Weather: Users can access hourly weather updates to plan their outfits accordingly. 
Wardrobe Management: In the wardrobe tab, users can add new clothing items or edit existing ones to build their virtual wardrobe. 

APIs / External Dependencies: 
Weather Data: The app retrieves daily weather forecasts from the Weatherbit.io API, which allows a maximum of 500 calls per day. Background Removal: We use the 
"GabrielBB/Android-CutOut" package to remove
backgrounds from user-uploaded clothing item images, ensuring a cleaner appearance. 

How Outfit Selection Works: 
The core of "WhatToWear" is its outfit selection algorithm, which is based on the concept of "clo" (thermal comfort unit). Here's how it works: 

Clo Model: The app uses the clo model of clothing thermal comfort, where 1 clo corresponds to the insulation needed to keep a person comfortable at rest in a room at 21 °C (70 °F) with specific conditions. 
Mapping Apparent Temperature: The app maps apparent temperature to clo units based on a reference image, helping determine suitable outfit insulation for the day's weather. 
Calculating Clo for Clothing Items: For user-entered clothing items, the app estimates clo values using a simplified model based on fabric's thermal conductivity, weight, and fabric blend information. While this model simplifies heat transfer considerations, it serves the purpose of recommending outfits effectively. 
Outfit Clo Value: The app calculates the clo value of complete outfits, considering the clo values of individual clothing items. The clo value of an outfit is determined by summing the clo values of its components, scaled by a factor of 0.82. 
Outfit Recommendations: The app generates outfit recommendations by searching for combinations of top, bottom, and outerwear that have a clo value closest to the desired clo value for the current day's temperature. This ensures users are dressed comfortably.
Submission: 

This submission reflects my experience and activities during the development of the "WhatToWear" Android app. It includes the following components: 

Description of Project: I have developed the "WhatToWear" Android app, focusing on outfit recommendations based on daily weather forecasts. The app also includes features like hourly weather updates and wardrobe management. 

References: 
Weatherbit.io API: Used for retrieving daily weather forecasts. 
GabrielBB/Android-CutOut Package: Utilized for background removal from clothing item images.

GitHub Repository: Contains the code for the Android app. 

Development Process: I followed these steps during the development process: Installed Android Studio and watched introductory tutorials to get familiar with Android app development. Built a weather app that accepts user input for location and fetches weather data from the Weatherbit API. Implemented version control using Git and documented my work, tasks, and progress. Set up a Firebase backend service to store user preferences and clothing items, enabling communication via a RESTful API. Collaborated with my partner, [Partner's Name], to coordinate code changes and debug issues. 

Screenshots: Link to App Screenshots 

GIT History: GitHub Repository - Commits

Reflection: Working on this assignment was a valuable experience in Android app development, API integration, and collaboration. I gained proficiency in Android Studio, implemented API calls for weather data, and successfully coordinated with my partner. We encountered challenges, particularly with user authentication, but resolved them effectively. This assignment has enhanced my confidence in mobile app development, and I look forward to exploring this field further in the course.
