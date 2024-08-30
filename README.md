# Online Visitor Counter

This project is an online visitor counter that uses Firebase to track and display the number of active users in real-time. The project includes HTML, CSS, and JavaScript files, with Firebase managing the real-time data updates.

## Project Structure

- `index.html`: The main HTML file for the project.
- `styles.css`: The CSS file for styling the webpage.
- `script.js`: The JavaScript file for handling Firebase configuration and real-time updates.
## Replace Following
// Your web app's Firebase configuration
const firebaseConfig = {
  apiKey: "YOUR_API_KEY_HERE",
  authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
  databaseURL: "https://YOUR_PROJECT_ID.firebaseio.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT_ID.appspot.com",
  messagingSenderId: "YOUR_SENDER_ID",
  appId: "YOUR_APP_ID",
  measurementId: "YOUR_MEASUREMENT_ID"
};
// Initialize Firebase
firebase.initializeApp(firebaseConfig);

## Realtime Rules
``` {
  "rules": {
    ".read": false,
    ".write": false,
      "tempUser":{
        ".read":true,
         ".write":true,
         ".indexOn":"state"
      }
  }
} 
