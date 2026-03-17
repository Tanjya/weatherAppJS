# Weather App - DataOps

## Description
This project is a simple backend **Weather API application** built with Node.js and Express.  
It fetches weather data from an external API and stores the results locally.

The app demonstrates **DataOps principles** by automating the collection, storage, and logging of weather data.

The system retrieves weather information, saves the latest data in a JSON file, and logs historical weather updates in a CSV file.

---

## Features
- Fetches live weather data from an external API
- Stores the latest weather data in a JSON file
- Logs weather history in a CSV file
- Provides API endpoints to access weather data
- Serves a simple frontend from the `public` directory

---

## Technologies Used
- Node.js
- Express.js
- OpenWeather API
- CSV Parser
- dotenv
- File System (fs)

---


---

## Installation

1. Clone the repository
On your termninal:
2. `cd` to root folder
3. Create a `.env` file with:
    `WEATHER_API_KEY`=your_api_key_here
    `CITY`=of your choosing
    `PORT`=of your choosing
4. `npm install` to install dependencies
5. `node fetchWeather.js` to create/update data folder
6. `node app.js` to start server
open browser on `PORT` to see weather app

## Using docker
1. Open your docker desktop
Make sure you are on the same path as dockerfile
On your terminal run:
2. `docker build -t <app-name>:<tag> . ` or `docker build -t weatherapp:1.0 .` to build an image based on dockerfile
3. `docker run -p <local-port>:<container-port> <image-name>` or `docker run -p 3000:5000 weatherapp` to run a container based on an image
