# Drone-Implementation

Server &amp; client implementation for the multi-drone master's project

Structure based on the following create, retrieve, update and delete (CRUD) example: https://testdriven.io/blog/developing-a-single-page-app-with-flask-and-vuejs/#put-route

# Dependencies

- Vue v2.6.11
- Vue CLI v4.5.11
- Node v15.7.0
- npm v7.4.3
- Flask v2.1.0
- Python v3.9.1

# Setup

Initial setup

- Install Python 3.9.X
- Install Node.js
- In a global admin CMD: npm install -g @vue/cli
- Install VSCode
- In VSCode, install the Prettier Extension
- In VSCode, go to File -> Preferences -> Settings, search for editor: format on save and check it on. Then, search for editor: default formatter and set the default formatter to Prettier
- Open the project folder with VSCode
- Always make shure to set VSCode to LF and not CRLF! (you can see the option at the bottom of VSCode)

Create a virtual environment:

- In a new Terminal
- Open an admin CMD in the project folder
- cd server
- pip install pipenv
- pipenv shell
- pip install Flask==2.1.0 Flask-Cors==3.0.10
- python app.py
- Backend should now be reachable under http://localhost:5000/ping
- To stop server, press Ctrl + C in terminal

Fire up development server

- In a new Terminal
- cd client
- npm run serve
- Client should now be reachable under http://localhost:8080
- You can click the errors away in the top-right. Errors shouldn't appear if you set up VSCode correctly with Prettier and made sure that every file is LF and NOT CRLF.

# Structure Client/Frontend

The client/public/index.html file is the starting point of our Vue application.

The client/src/router/index.js file describes the routers of the frontend.

The client/src/components directory contains different .vue files. The .vue files are single file components which are broken up into three different sections:

1. template: for component-specific HTML
2. script: where the component logic is implemented via JavaScript
3. style: for CSS styles

The client/src/App.vue file is the root .vue file into which the other .vue files will be inserted when the frontend is displayed.

# Structure Server/Backend

Everything is handled in the server/app.py file.
