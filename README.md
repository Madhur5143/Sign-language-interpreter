# Sign Language Video Call Interpreter

This project is a **real-time sign language interpretation web application** that integrates **video calling** with **AI-based gesture recognition**. It allows two users to connect through a peer-to-peer video call while automatically detecting hand gestures and converting them into readable text for the other participant.

The application uses **WebRTC via PeerJS** for real-time communication and **MediaPipe Gesture Recognition** to analyze hand movements captured by the webcam. When the interpreter is enabled, the system processes video frames in real time, detects gestures, and sends the interpreted text to the connected user through a data channel.

Recognized gestures are displayed as a **text overlay on the video stream**, enabling easier communication between sign language users and non-signers during the call.

## Features

- Real-time **peer-to-peer video calling**
- **AI-powered gesture recognition** using MediaPipe
- **Live text interpretation** overlay during calls
- Ability to **toggle the interpreter on/off**
- **Unique Peer ID** generation for connecting users
- **Incoming call handling** (accept, reject, end call)
- Clean and responsive interface built with **Tailwind CSS**

## Technologies Used

- HTML5
- JavaScript (ES Modules)
- Tailwind CSS
- PeerJS (WebRTC communication)
- MediaPipe Tasks Vision (Gesture Recognition)

## Requirements

- Modern browser (Chrome, Edge, or Firefox)
- Webcam and microphone access
- Local PeerJS signaling server

## Running the Project

1. Start a PeerJS server:

```bash
npx peerjs --port 9000
