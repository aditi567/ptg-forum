
PTG Forum🤝
---
A web portal that allows students to post their issues anonymously.
***
Technologies used : 
---
1) NodeJS 
2) ExpressJS
3) MongoDB
4) Mongoose
5) Google authentication API
6) Passport
***

🧾Pre-requisite :
---
1) Run the following command to install all the dependencies listed in the package.json file:

```javascript
npm install
```

2) Create .env file to store your credentials od google authentication API -- Update GoogleStrategy callBackURL in app.js
3) Create your Mongo Atlas cluster for the cloud DB and Update its link in app.js
4) Time is configured as en-IN
5) The app is configured for deployed port as well as port 8000 on localhost.
6) To run on localhost
```
node app.js
```
***
✨Flow of application :
---
1) Portal of anonymous messages is visible along with their timestamp at : <pathToWebsite>/messages
2) If user wants to message then user will be directed to sign up using their email and create password credential or they can sign up through google.
-- If user already exists then log in directly using credentials or through google.
3) The login session will be alive until the browser window is closed.
4) User can submit messages at /submit route provided their login session is alive.