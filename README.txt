🌟 Chat App

Project Overview

The Chat App is a Flutter-based project utilizing OpenAI's GPT-3.5 API to create an interactive chatbot experience. This application allows users to:✅ Start new conversations✅ View chat history✅ Mark chats as favorites✅ Refresh conversations anytime

📌 System Requirements

Operating System: Windows, macOS, or Linux

Flutter SDK: Version 3.0 or later

Dart SDK: Included with Flutter SDK

API Key: OpenAI API key to enable chatbot functionality

🚀 Setup Instructions

Step 1: Clone the Repository

Open a terminal and navigate to the desired directory, then clone this repository:

git clone <repository-url>
cd chat_app_project

Step 2: Install Dependencies

Ensure that Flutter is installed by running:

flutter doctor

This will confirm that Flutter and Dart SDKs are set up correctly.

Then, install the required dependencies:

flutter pub get

Step 3: Configure OpenAI API Key

Open lib/contact_page.dart and locate the apiKey variable.Replace the placeholder value with your OpenAI API key:

final String apiKey = 'YOUR_OPENAI_API_KEY';

Step 4: Add Assets

Ensure the following directory structure in your project:

assets/
├── chatgpt.jpg
├── nghia.jpg
├── long.jpg
└── thang.jpg

Add these references to your pubspec.yaml:

flutter:
  assets:
    - assets/chatgpt.jpg
    - assets/nghia.jpg
    - assets/long.jpg
    - assets/thang.jpg

Step 5: Run the Application

Run the app on an emulator or connected device:

flutter run

If using an IDE (Android Studio/VSCode), select the device before running.

🛠 Feature Testing

✅ Testing Chat Functionality

Start a New Chat – On the Home screen, type a message to start a conversation with the chatbot. Ensure the response is displayed.

View Chat History – Open the chat history from the drawer menu and verify previous conversations.

Favorite a Chat – In the chat history, tap the heart icon to mark a conversation as a favorite, then check if it's saved.

Refresh the Chat – Return to the main screen and tap the refresh icon to start a new conversation.

📌 Notes & Additional Information

A stable internet connection is required for responses from the OpenAI API.

Tested on Flutter 3.0.0, Android 10, and iOS 14 simulators (compatibility may vary).

Ensure all assets in the assets/ folder are correctly referenced.

