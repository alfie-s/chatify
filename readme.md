# Chatify

A web chat app that you can talk to other users who are signed in. You can also create group chats and admins can remove users from group chats.

## This app was created using MongoDB, Expressjs, Reactjs, Nodejs, Chakra UI for css components and Socket IO for real time messaging(although it does not seem to work on the deployed site if you try to open two browser windows on the same computer).

# Live deployment

I am not sure if it needed deployment for this task as heroku is not available but I have tried to deploy to Render.

You can view the deployed app here: https://chatify-b5yp.onrender.com

Best way of testing this app is to open it on your phone as well as your desktop and sign in with two different users and start a chat.

I have tried to make it as responsive as I can in the timeframe, but it is still not 100% optimised for phone.

As mentioned above - There are some issues with real time messaging on Render and the chat list takes some time to load also. I haven't found a resolution at this time. real time chat messages take abot 5 seconds to come through.

log in with a name email password and profile picture.

There are some test accounts to chat with, or you can make more than one account yourself.

# Deploying Locally

This app works well locally

- download or clone this git repo
- set up your own .env file with mongodb credentials and secret key for JWT
- npm install on both the backend and frontend folders.
- npm start on both the backend and frontend folders.

# System Architecture Overview

The chat app will be a web-based application that allows users to communicate with each other in real-time through a web browser on desktop and mobile devices. The app will consist of a client-side interface that runs in the user's web browser and a server-side component that handles data storage, processing, and transmission. The chat app will be

## Client-side Components

The client-side interface of the chat app will be implemented using HTML, CSS, and JavaScript, using React.js as the front end of the MERN stack. It will be responsible for rendering the user interface, handling user input, and making requests to the server as needed.

### The client-side interface will consist of the following modules:

- Passport Authentication module: This module will handle user login and registration with a valid Google or Facebook account, as well as a valid email address.
- Chat module: This module will be responsible for rendering the chat interface and handling all communication with the server. It will allow users to send and receive messages and emojis.
- Admin Chat module: This module will render the modal allowing the user to create new chats and invite users to the chat. This will also allow the user to become admin and remove users from the selected chat and change the chat name.
- Notification module: This module will handle real-time notifications for events such as new messages and group invites.
- List Module: This module will allow users to view their current list of groups and one to one chats.

## Server-side Components

The server-side component of the chat app will be implemented using MongoDB, Express and Node as part of the MERN stack. It will be responsible for storing and processing data, as well as handling requests from the client-side interface.

### The server-side component will consist of the following modules:

- Authentication module: This module will handle user authentication and session management. It will validate user login credentials and manage user sessions to ensure secure access to the app.
- Chat module: This module will handle all communication between users, including sending and receiving messages, creating and managing groups, and sharing files. It will also handle real-time updates and notifications.
- Data storage module: This module will handle data storage and retrieval, using a database management system MongoDB.

### Software Requirements Document

1. Introduction

- Purpose:
  - The purpose of this document is to specify the requirements for a web-based chat app that allows users to communicate with each other in real-time.
- Scope:
  - The scope of this project includes the development of a web-based chat app that allows users to send and receive messages, create and join group chats, and share files. The app will be accessible through a web browser on desktop and mobile devices.
- Definitions, acronyms, and abbreviations:
  - Chat app: A web-based application that allows users to communicate with each other in real-time.
  - MERN stack: A web development framework, consisting of front, middle and backend technologies that enables faster development when creating web based applications. A MERN stack has MongoDB, ExpressJS, ReactJS and NodeJs as its working components.

2. Overall Description

- Product perspective: The chat app will be developed as a standalone product that can be accessed through a web browser.
- User characteristics: The chat app will be used by a wide range of users wanting to use a chat application who would like the option of group or one on one chats.
- Operating environment: The chat app will be accessed through a web browser on desktop and mobile devices.
- User interface: The chat app will have a simple and intuitive user interface that allows users to easily navigate the app and communicate with each other.

3. User Stories

- As a user, I want to be able to send and receive real-time messages to and from other users so that I can communicate with my friends and colleagues.
- As a user, I want to be able to create and join groups for group communication so that I can communicate with a larger group of people.
- As a user, I want to be able to share files within chats and groups so that I can easily share documents and other resources.
- As a user, I want to be able to see when other users are online or offline so that I know when they are available to chat.
- As a user, I want the chat app to have a simple and intuitive user interface that is easy to use so that I can easily navigate and use the app.
- As a user, I want the chat app to support emojis and rich text formatting so that I can express myself more fully in my messages.

4. Specific Requirements

4.1 Functionality

- Users will be able to create an account and log in to the chat app.
- Users will be able to send and receive real-time messages to and from other users.
- Users will be able to create and join groups for group chats.
- Admins of group chats will be able to edit the group chat name and remove users from group chat.
- Users will receive notifications if not in a chat.
- Users will be able to customise their profile picture.
- The chat app will support emojis.

  4.2 Performance

- The chat app will have a response time of less than 2 seconds for all actions.
- The chat app will support up to 10 concurrent users.

  4.3 Security

- The chat app will use secure servers and encrypt all data transmitted between the client and the server.
- The chat app will support secure login using passwords.

  4.4 Compatibility

- The chat app will be compatible with the latest versions of major web browsers, including Google Chrome, Mozilla Firefox, and Microsoft Edge.
- The chat app will be compatible with mobile devices running iOS and Android.

  4.5 Usability

- The chat app will have a simple and intuitive user interface that is easy to use for all users.
- The chat app will provide clear and concise instructions for all actions.

  4.6 Reliability

- The chat app will have 99.9% uptime.
- The chat app will recover from failures and errors without losing data.

5. External interfaces

- The chat app will be accessed through a web browser on desktop and mobile devices.
- The chat app will use secure servers for storing and processing data.

6. Constraints

- The chat app must be developed using web technologies, such as HTML, CSS, and JavaScript, using the MERN stack
- The chat app must be compatible with the latest versions of major web browsers, including Google Chrome, Mozilla Firefox, and Microsoft Edge.
- The chat app must be compatible with mobile devices running iOS and Android.

7. Assumptions and dependencies

- It is assumed that users have a web browser and internet connection to access the chat app.
- It is assumed that users have an email address to create an account for the chat app.
- The chat app will depend on secure servers for storing and processing data.
