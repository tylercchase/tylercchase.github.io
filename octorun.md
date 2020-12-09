---
layout: post
title: OctoRun
description: My computer security class final project
image: null
nav-menu: true
show_tile: true
---

(tl;dr) : A service for running code on the web using angular,express, and docker

# Frontend
The frontend itself is written in [angular](https://angular.io/) and uses the [monaco editor](https://microsoft.github.io/monaco-editor/) to display the code written by the user. 
## Angular
I picked angular because it's what I am most familiar with, but you would be able to use any framework or none at all if you want.

# Backend
The backend is written in [express](https://expressjs.com) and uses [passport.js](http://www.passportjs.org/) to do Google OAuth 2.0.

## MongoDB
An easy to use NoSQL database. It was my first time using it, and it was an enjoyable experience. I used [mongoose](https://mongoosejs.com/)
## Passport
Passport is awesome, in that, it lets you select from a variety of different "strategies" or ways to log in. For this project, I selected the Google Oauth 2.0 strategy, but could easily integrate other platforms to log in with.
# Manager
The manager script is written in python and uses flask.
The manager is using the python [docker SDK](https://docker-py.readthedocs.io/en/stable/) to manage docker containers on the server.
In the future, I would ideally want to remove the manager-script and rely on something like Kubernetes to keep the client code off of my server. For this project though I decided to use this since I was familiar with python more than Kubernetes, and wasn't sure if it was going to be the right solution.

