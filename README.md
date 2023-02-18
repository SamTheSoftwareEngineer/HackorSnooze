# HackorSnooze

You will see that stories are displayed and there is functionality to log in and create a user. This code also includes features to let users add new stories, favorite a story, and delete a story.

The front-end app consists of two parts:

Classes and methods for the big data ideas: a Story class for each story, a StoryList class for the list of stories, and a User class for the logged-in user (if any). These methods also handle interacting with the API.
Functions for the UI, handling things like reading form values from forms and manipulating the DOM.
Separation of Concerns and Organization

We’ve divided the code up into those different parts for readability and maintenance. It’s often useful to think about the data and the UI separately, (a separation of concerns). Many apps are written this way.

There’s one JS file for the “data” layer of the app:

js/models.js
contains classes to manage the data of the app and the connection to the API. The name models.js to describe a file containing these kinds of classes that focus on the data and logic about the data. UI stuff shouldn’t go here.

Read this file thoroughly. There is a new keyword here, static. Make sure you understand what it means before moving on.

For the UI layer, we’ve broken this into several files by topic:

js/main.js
contains code for starting the UI of the application, and other miscellaneous things.

js/user.js
contains code for UI about logging in/signing up/logging out, as well as code about remembering a user when they refresh the page and logging them in automatically.

js/stories.js
contains code for UI about listing stories.

js/nav.js
contains code to show/hide things in the navigation bar, and well as code for when a user clicks in that bar.

This image helps to conceptualize the way the functions interact within this code:
![image](https://user-images.githubusercontent.com/20036100/219904532-e0c07aef-93f9-4303-86f2-aa5b0d279fa7.png)


**Further Study**
1. Add some error handling for when a username has already been taken or if credentials are incorrect!
2. Allow users to edit stories they have created.
3. Add a section for a “user profile” where a user can change their name and password in their profile.
4. Style the application so that it is presentable on mobile devices.
5. Add infinite scroll! When a user scrolls to the bottom of the page, load more stories.
6. Come up with some other features you can build using what our Hack or Snooze API makes available to you!


