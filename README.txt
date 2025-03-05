
1. Project Overview
The Chat App is a Flutter-based project utilizing OpenAI's GPT-3.5 API to create an interactive chatbot experience. This application allows users to start new conversations, view their chat history, mark chats as favorites, and refresh the conversation anytime.

2. System Requirements
Operating System: Windows, macOS, or Linux
Flutter SDK: Version 3.0 or later
Dart SDK: Included with Flutter SDK
API Key: OpenAI API key to enable chatbot functionality
3. Setup Instructions
Step 1: Clone the Repository
Open a terminal and navigate to the desired directory.
Clone this repository:
bash
Copy code
git clone <repository-url>
Navigate into the project folder:
bash
Copy code
cd chat_app_project
Step 2: Install Dependencies
Ensure that Flutter is installed by running:

bash
Copy code
flutter doctor
This will confirm that Flutter and Dart SDKs are set up correctly.

Install the necessary dependencies:

bash
Copy code
flutter pub get
Step 3: Configure OpenAI API Key
Open lib/contact_page.dart and locate the apiKey variable.
Replace the placeholder value with your OpenAI API key:
dart
Copy code
final String apiKey = '';

Step 4: Add Assets
In the project directory, locate the assets/ folder. Add any required images (such as profile pictures and logos) to this folder. Ensure the following structure:
arduino
Copy code
assets/
├── chatgpt.jpg
├── nghia.jpg
├── long.jpg
└── thang.jpg
Confirm these assets are referenced in the pubspec.yaml file. Open pubspec.yaml and ensure the following lines are added:
yaml
Copy code
flutter:
  assets:
    - assets/chatgpt.jpg
    - assets/nghia.jpg
    - assets/long.jpg
    - assets/thang.jpg
Step 5: Run the Application
To run the app on an emulator or connected device:
bash
Copy code
flutter run
Select the device in your IDE (Android Studio or VSCode) if you’re not using the command line.

4. Feature Testing
Testing Chat Functionality
Start a New Chat: In the app’s main (Home) screen, type a message to initiate a conversation with the chatbot. Confirm that the app displays the AI’s response.
View Chat History: Access the chat history page from the drawer menu and ensure previous conversations appear with the correct messages.
Favorite a Chat: In the chat history, mark a conversation as a favorite by tapping the heart icon, then verify the status in the list.
Refresh the Chat: Return to the main screen and click the refresh icon to start a new conversation.

5. Notes and Additional Information
Ensure you have a stable internet connection to receive responses from the OpenAI API.
Tested on Flutter version 3.0.0, Android 10, and iOS 14 simulators. Compatibility may vary with other OS versions.
The project uses assets located in the assets/ folder for contact avatars and logos, so ensure these are correctly referenced.
