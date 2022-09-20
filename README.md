# drone-implementation

Server &amp; client implementation for the multi-drone master's project

Structure based on the following create, retrieve, update and delete (CRUD) example: https://testdriven.io/blog/developing-a-single-page-app-with-flask-and-vuejs/#put-route

# dependencies

- Vue v2.6.11
- Vue CLI v4.5.11
- Node v15.7.0
- npm v7.4.3
- Flask v2.1.0
- Python v3.9.1

# setup

Create a virtual environment:

- Open an admin CMD in the project folder
- cd server
- pip install pipenv
- pipenv shell
- pip install Flask==2.1.0 Flask-Cors==3.0.10
- python app.py
- Backend should now be reachable under http://localhost:5000/ping
- To stop server, press Ctrl + C in terminal

Vue Setup

- Install Node.js
- In a global admin CMD: npm install -g @vue/cli
- npm install --save-dev eslint eslint-plugin-vue
- Within the project folder (the one with server & frontend) run: vue create client
- npm install axios@0.21.1 --save
- npm install bootstrap@4.6.0 --save

Fire up development server

- cd client
- npm run serve

# Structure

The index.html file is the starting point of our Vue application.

.vue files are single file components which are broken up into three different sections:
1.) template: for component-specific HTML
2.) script: where the component logic is implemented via JavaScript
3.) style: for CSS styles
