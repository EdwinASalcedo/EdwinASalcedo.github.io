---
title: "LiftLog Dev Status 1"
date: 2025-07-06T06:00:23+06:00
description: Developer status update on LiftLog
theme: Toha
menu: 
    sidebar:
        name: Dev Status 1
        identifier: liftlog-dev-status-1
        parent: liftlog
        weight: 10
---
### Why

I am building this app as a way to test myself on what I have learned from the 100 Days of SwiftUI course from HackingWithSwift. And what better way to do it than by trying to emulate an app I use everyday, 'Strong' on the AppStore. As of right now I just want to be able to do the basics such as starting a workout, input exercises, save templates, have set timers, and add new exercises. The app I am basing it off of has much more functionality than that but this is what I am currently aiming for.

### Future

In the future I want to be able to come back to this project and improve upon it and make it into something of my own with different styling and features. A promising feature I recently saw from Apple is the on device foundation models coming in iOS 26. I would like to use this feature to where users can ask the model to structure a workout for them by providing a template for them based on the user's needs. Once I start actually making the app my own I would like to release it on the AppStore and get real user feedback on how the app can improve and what bugs they encounter so that I can fix them.

### Current Progress
{{< img src="images/example3.png" height="350" float="right" title="Example3">}}
{{< img src="images/example2.png" height="350" float="right" title="Example2">}}
{{< img src="images/example1.png" height="350" float="right" title="Example1">}}

As of right now the app has the functionality to quick start a workout which will display a WorkoutView in a sheet. Within this WorkoutView users will be able to choose which exercises they want to add. Another option is that users can instead start a workout from a saved template. I will provide some default templates but users will be able to create and save their own. 

In the WorkoutView users will be able to set a timer between their sets which can also be disabled. As you can see you can input the weight and sets done for the exercise. Once the user has finished their set they can tap on the checkmark button to set it as done which will tint the row green. While I have not implemented the timer yet, the idea is that it will start once the set is marked as done and once the timer finishes I will utilize the new Alarmkit features coming in iOS 26. 

As of right now I still need to be able to log the workout as complete when the user taps 'Finish' on the upper right corner. With workouts being saved the user will be able to view past workouts and even turn a workout into a new template for future use.

I have another view that I just finished up and it is the ExerciseView. Within the ExerciseView users will be able to see all of the available exercises they can choose from. In the upper left corner users will be able to add in their own exercises and these are saved and persisted throuhgout the app. Users can also filter through the exercises based on body part, category, search, or all combined! As of right now I do not provide images for the exercises but I may include some for common exercises in the future. I am contemplating on letting users add their own images for exercises but this is a feature I would have to think about later.

Thats it for this update!