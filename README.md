# Free City Hub

Free City Hub is your portal into all apps and services that is available on the Free City Platform

## Portal to your Free Life

The Hub integrates many different apps and services, collecting and aggregating a view of all your data that belongs to you and your decentralized identity (DID).

![](/assets/free-city-hub-screenshot.png)

## Get Started

To start developing on this repository, open two instances of your terminal app. One should navigate into the `server` folder and another into the `app` folder. Ensure that you run `npm install` on both folders and then you can run `npm start` on both to start both the API server and the UI.

Angular (hot-reload): http://localhost:4200/  
Server (API and UI hosted together): http://localhost:5050/

You also need an instance of MongoDB running on your local machine, preferbly through Docker. You can create a file named `.env` within the `server` folder that contains the connection string to your MongoDB database. The `.env` file should not be committed to source control.

```
HUB_DATABASE=mongodb://localhost:27017
PORT=5050
```

## Authentication on `localhost`

If you want to use the authentication mechanism with cookies on localhost, you need to run production build of the UI and access the web app through the singular port that hosts both UI and API on same ports (5050).
