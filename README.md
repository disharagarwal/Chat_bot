# ChatBot Component

The ChatBot component is a simple chat interface that allows users to interact with a bot and provide inputs in the form of text or voice. It presents a series of predefined questions to the user and collects their responses. The collected inputs can then be displayed and saved to a server.

## Technologies Used

- React: A JavaScript library for building user interfaces.
- Axios: A popular HTTP client library for making API requests.
- SpeechRecognition API: Used for voice recognition in supported browsers.
- Mysql for backend

## Getting Started

To use the ChatBot component in your project, follow these steps:

1. Install the required dependencies by running the following command:
npm install axios


2. Create a new file called `ChatBot.js` and copy the code of the ChatBot component into it.

3. Import the `ChatBot` component into your desired file where you want to use it.

4. Place the `<ChatBot />` component in your JSX code to render the chat interface.

## Usage

The ChatBot component provides a chat interface where the user can input their responses to the predefined questions. It supports both text and voice input.

The component maintains a conversation flow by displaying questions one by one and collecting the user's responses. Once all the questions are answered, the collected inputs are displayed and can be saved to a server.

### Available Functions

The ChatBot component provides the following functions:

- `startVoiceRecognition()`: Starts voice recognition to capture user input using the device's microphone.
- `stopVoiceRecognition()`: Stops the voice recognition process.
- `handleUserInput(event)`: Handles the user's input, whether from text or voice, and updates the state accordingly.
- `handleVoiceInput(event)`: Handles the voice input and updates the `voiceInput` state with the captured transcript.

### Configuration

The ChatBot component utilizes an array of predefined questions and corresponding fields. You can customize this array by adding or removing questions to fit your use case. The questions are defined in the `questions` array inside the component.

### Styling

The component uses a CSS file named `style.css` to apply styles to the chat interface. You can modify this file or add your own styles to customize the appearance of the chat interface.

### Server Integration

The component includes an example of sending the collected user inputs to a server using the `axios` library. The code uses a POST request to send the data to `http://localhost:3001/save`. You can update this URL to match your server endpoint or modify the code to integrate with your specific server implementation.



