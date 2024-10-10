# OpenAI Realtime API Demo

This project demonstrates a real-time interaction with OpenAI's GPT-4o model using WebSockets. It consists of a React frontend and a Node.js backend that connects to OpenAI's Realtime API.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project showcases a real-time chat application that interacts with OpenAI's GPT-4o model. Users can send audio messages, which are processed and responded to by the AI in both text and audio formats. The application is built with a React frontend and a Node.js backend, utilizing WebSockets for real-time communication.

## Features

- **Real-time Communication**: Uses WebSockets to maintain a persistent connection between the client and server.
- **Audio Processing**: Records audio from the user's microphone, processes it, and sends it to the backend.
- **AI Interaction**: Connects to OpenAI's Realtime API to receive AI-generated responses in text and audio.
- **Automatic Audio Playback**: Plays audio responses automatically using a hidden audio player.

## Installation

### Prerequisites

- Node.js and npm installed on your machine.
- A valid OpenAI API key.

### Steps

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/openai-realtime-api-demo.git
   cd openai-realtime-api-demo
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Set up environment variables**:
   Create a `.env` file in the root directory and add your OpenAI API key:
   ```plaintext
   OPENAI_API_KEY=your_openai_api_key
   ```

4. **Start the backend server**:
   ```bash
   node backend/server.js
   ```

5. **Start the frontend**:
   ```bash
   npm start
   ```

## Usage

- Open your browser and navigate to `http://localhost:3000`.
- Click the "Start Recording" button to begin recording your message.
- Click "Stop Recording" to send the message to the AI.
- The AI's response will be displayed in text and played back in audio.

## Project Structure

- **src/App.js**: The main React component handling UI and WebSocket communication.
- **backend/server.js**: Node.js server that connects to OpenAI's Realtime API and handles WebSocket communication with the client.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.