# BikeUi

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 7.3.8.

The purpose of this project is to serve as the front-end for my bike registration app, which communicates to Spring Boot (the backend).

## Service Calls
I started out by finishing the API calls to the Spring Boot server by adding some service calls to the bike.service file.

## Added home component and form
Once that was in place I could then create the home component that would accept the user registration via an html form. This was a little different because I needed to accept user input, do a validation and handle posting the contents back to Spring Boot.

## Added view registration component
I then added another component to handle viewing a specific registration and tied that into the admin list screen.

## Add Bootstrap and custom CSS
To make everything start to look a little more pleasant, I then added some Bootstrap and some of my own custom styling to the application.

## Set up a production build
And finally, I developed a way how to run Angular in a production environment by using a Node Express server and running the production build using the Angular CLI Build Tool.
