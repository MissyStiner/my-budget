# My Budget | Budget Tracker

## GitHub URL
https://github.com/MissyStiner/my-budget

## Application URL


## User Story
AS AN avid traveler<br>
I WANT to be able to track my withdrawals and deposits with or without a data/internet connection<br>
SO THAT my account balance is accurate when I am traveling 

## Acceptance Criteria
GIVEN a budget tracker without an internet connection<br>
WHEN the user inputs an expense or deposit<br>
THEN they will receive a notification that they have added an expense or deposit<br>
WHEN the user reestablishes an internet connection<br>
THEN the deposits or expenses added while they were offline are added to their transaction history and their totals are updated

## Mock-Up
![image](https://user-images.githubusercontent.com/85651869/140235331-e2a34c62-9294-40e0-8cf0-568304a5f456.png)

## Offline Functionality
You’ll need to use IndexedDB to add offline functionality. Review Module 18: NoSQL, Lesson 4: Add Offline Persistence with IndexedDB as a refresher on how to add this to your application.

You’ll also need to add a service worker to your application. Review Module 19: Progressive Web Applications (PWA), Lesson 4: Using Service Workers as a refresher on how to add this to your application.

### Rewind
The Food Festival application that you created in this module's lessons did not include an Express.js server, so you used the webpack-dev-server npm module to test the service worker with an HTTPS-enabled server.

For this Challenge, however, you aren't using webpack, but you do have an Express.js server provided to you in the starter code. Remember that Chrome DevTools makes it possible to test service workers on localhost in development. Simply click the Application tab, then select Service Workers from the menu on the left.

# Important
You should add your idb.js file to the public/js/ directory of your application.

You should add your service worker to the root of the public/ directory of your application.

Once you’ve updated the existing budget tracker, it should provide the following functionality:

- The ability to enter deposits offline.

- The ability to enter expenses offline.

- Offline entries should be added to the tracker when the application is brought back online.

## Web Manifest
Because this will be a mobile-first application, you’ll also need to add a web manifest to your application with the app’s metadata, to let users’ devices know what they’re installing and how the app should look on the home screen.

This manifest.json file for this project will contain the following properties:

- name

- short_name

- icons

- theme_color

- background_color

- start_url

- display

In the module project, you used webpack to create the manifest.json file. For this application, you’ll need to create it manually and add it to the root of the public/ directory of your application. You can also review Module 19: Progressive Web Applications (PWA), Lesson 5: Convert the App to a PWA as a refresher on web manifests.

## Deployment to Heroku Using MongoDB Atlas
Finally, the budget tracker has a server and uses MongoDB as its database, so you’ll need to deploy this application to Heroku using MongoDB Atlas. To review this process, look at Module 18: NoSQL, Lesson 5: Add Mongoose Validation, specifically 18.5.5: Deploy to Heroku.
