# connect
A real-time chat application.


## Visual Demo
(no sound)

https://user-images.githubusercontent.com/71296308/216512071-5d5d8fea-1001-44f0-9247-a61ac24b48fe.mp4


## Overview
Visit: https://davmoba4.com/project/connect/


## How to Run Locally
### Backend
- Navigate to the **server** folder on the terminal and run the following command to install the dependencies:
``` 
npm install
```
- Create a .env file inside your **server** folder and store the following variables inside:  
 PORT = < port number for your server ( e.g. 5000 ) >  
 CORS_URL = < your frontend's URL ( e.g. http://localhost:3000 ) >  
 MONGO_URI = < the URI connecting to your MongoDB database >   
 JWT_SECRET = < the secret string used to create and verify your tokens (can be anything) >  
- Navigate to the **server** folder on the terminal and run the following command to start the backend:
```
npm start
```

### Frontend
- Navigate to the **client** folder on the terminal and run the following command to install the dependencies:
``` 
npm install
```
- Navigate to client/src/components/Chats/ChatBox.js. Then, on line 26, change the ENDPOINT variable to your server's URL.
- Navigate to client/package.json and change the "proxy" value to your server's URL.
- Navigate to the **client** folder on the terminal and run the following command to start the frontend:
```
npm start
```

## Acknowledgments
- Based and extended from: [mern-chat-app](https://github.com/piyush-eon/mern-chat-app).

### Some Features I've Added
- Guest account creation.
- Dark mode and light mode.
- Send button.
- Time stamps.
- Read receipts.
- Emoji selection.
- Real-time update of new message text preview.
- Ability to change the group admin.
- Ability to message someone from group by clicking their name.
