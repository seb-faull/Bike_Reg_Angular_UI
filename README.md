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

## Auth0
I needed an authentication service so I began by creating an Auth0 account. This allowed me to set up an OAuth secured app. If I were working for a large corporation I most likely will build this piece on my own and not use a third-party provider like Auth0.

## Spring Boot security dependencies and configuration
I then added security support to the Spring Boot server by adding the security dependencies and configuration needed so that I can receive and check tokens with Auth0.

## Angular security dependencies and configuration
Next I added the Angular client security dependencies and configuration.

## Callback component and authorisation service
And once all of that was in place I could then create my security callback component and set up the authorisation service so that I can initiate logins to Auth0 and receive notifications once the login has succeeded, which is known as the callback.

## Secure admin routes and pass the bearer token
Finally, I needed to secure the admin portion of the application and make sure that the secure API endpoint calls pass the bearer token so Spring Boot would grant access to that part of the API. I did that by creating the AuthGuard and by passing in the Authorisation Bearer on my API calls.
