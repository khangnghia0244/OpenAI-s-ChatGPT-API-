Chat App
1. Project Overview
The Chat App is a Flutter-based application leveraging OpenAI's GPT-3.5 API to provide an interactive chatbot experience. It allows users to initiate new conversations, review chat history, mark chats as favorites, and refresh conversations anytime.

2. System Requirements
Operating System: Windows, macOS, or Linux
Flutter SDK: Version 3.0 or later
Dart SDK: Included with Flutter SDK
API Key: OpenAI API key for chatbot functionality
3. Setup Instructions
Step 1: Clone the Repository
Open a terminal and navigate to your desired directory. Clone the repository using:

bash
Copy
Edit
git clone <repository-url>
Navigate into the project folder:

bash
Copy
Edit
cd chat_app_project
Step 2: Install Dependencies
Ensure Flutter is installed by running:

bash
Copy
Edit
flutter doctor
This will confirm that Flutter and Dart SDKs are correctly set up.

Next, install the necessary dependencies:

bash
Copy
Edit
flutter pub get
Step 3: Configure OpenAI API Key
Open lib/contact_page.dart and locate the apiKey variable.
Replace the placeholder with your OpenAI API key:

dart
Copy
Edit
final String apiKey = 'your_openai_api_key';
Step 4: Add Assets
Ensure the assets/ folder contains required images (e.g., profile pictures and logos). Your directory structure should be:

cpp
Copy
Edit
assets/
├── chatgpt.jpg
├── nghia.jpg
├── long.jpg
└── thang.jpg
Update pubspec.yaml to include these assets:

yaml
Copy
Edit
flutter:
  assets:
    - assets/chatgpt.jpg
    - assets/nghia.jpg
    - assets/long.jpg
    - assets/thang.jpg
Step 5: Run the Application
To run the app on an emulator or a connected device:

bash
Copy
Edit
flutter run
If using an IDE (Android Studio or VSCode), select the target device before running the app.

4. Feature Testing
Testing Chat Functionality
Start a New Chat: On the Home screen, send a message to begin a conversation with the chatbot. Verify that the AI responds correctly.
View Chat History: Navigate to the chat history page from the drawer menu and ensure past conversations display correctly.
Favorite a Chat: In the chat history, tap the heart icon to mark a conversation as a favorite. Check if it appears in the favorites list.
Refresh the Chat: Return to the main screen and tap the refresh icon to start a new conversation.
5. Notes and Additional Information
Ensure a stable internet connection for receiving responses from the OpenAI API.
Tested on Flutter 3.0.0, Android 10, and iOS 14 simulators. Compatibility may vary with different OS versions.
All required assets are located in the assets/ folder. Make sure they are referenced properly in pubspec.yaml.
