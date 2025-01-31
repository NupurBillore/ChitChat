# Chit Chat Application
A simple and scalable real-time chat application built with React for the frontend and Firebase for real-time database management. This application allows users to send and receive messages instantly with a seamless chat experience.

Features


Real-Time Messaging: Users can send and receive messages instantly with Firebase Realtime Database.

Authentication: Users can sign up and log in using Firebase Authentication (email/password or Google sign-in).

User Presence: Displays active users in the chat with the status indicator.
Responsive UI: Built using React and CSS for a user-friendly experience on both mobile and desktop.


Technologies Used
Frontend: React.js, React Router, Firebase, CSS

Backend: Firebase (Authentication, Realtime Database)

APIs: Firebase Authentication API, Firebase Realtime Database API

Deployment: Firebase Hosting

Firebase Setup
Create a Firebase project at Firebase Console.
Enable Firebase Authentication (Email/Password and/or Google Sign-In).
Set up Firebase Realtime Database in the "Database" section.
Copy your Firebase config object and create a .env file in the root directory with the following:

REACT_APP_FIREBASE_API_KEY=your-api-key
REACT_APP_FIREBASE_AUTH_DOMAIN=your-auth-domain
REACT_APP_FIREBASE_DATABASE_URL=your-database-url
REACT_APP_FIREBASE_PROJECT_ID=your-project-id
REACT_APP_FIREBASE_STORAGE_BUCKET=your-storage-bucket
REACT_APP_FIREBASE_MESSAGING_SENDER_ID=your-messaging-sender-id
REACT_APP_FIREBASE_APP_ID=your-app-id
Usage

Sign Up/Login: Use the Google sign-in option or create an account with email and password.

Chat: Once logged in, you can start chatting in the app, view messages in real-time, and see online users.

Firebase Realtime Database Structure
The Firebase Realtime Database structure is as follows:

typescript

/users
  /userId
    username: string
    email: string
    onlineStatus: boolean
/messages
  /chatId
    /messageId
      text: string
      senderId: string
      timestamp: number
