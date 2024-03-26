# Log dashboard

This is a simple application built using node and express to read the logfile, parse data and convert to json format and Vite and React to get the data from 'API' and display the data on the screen.

There are to small applications within the folder

- server
- frontend

## Running the application

In order to run the application both server and frontend need to be running. Follow the steps below to run the application.

- Navigate to server folder
- Run ```npm install``` to install dependencies for server
- Run ```npm start``` to start the server. This will run the application on port 3001
- Navigate to frontend folder
- Run ```npm install``` to install dependencies for frontend
- Run ```npm run dev``` to start the frontend app. This should server the app on http://localhost:5173/

## Considerations and next steps

- Currently the app takes a log file and converts that. This is a limitation as ideally we should be able to make this process more dynamic. A moire complete approach would be to create a frontend that allows user to upload a log file, that can then be passed to the server to decode/parse and then the frontend can generate a log report.
- The server is currently allowing any URL to access the server as cors is set to any. In a production mode, we would be limiting the interaction of server and frontend as exposing the server is a security risk.
- More tests are required specially in the frontend code and at component levels. As the application is simple and core logic is tested, snapshot tests should be sufficient.
