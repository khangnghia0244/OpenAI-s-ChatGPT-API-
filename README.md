# 📱 CHAT APP

## PROJECT OVERVIEW

The Chat App is a Flutter-based project utilizing OpenAI's GPT-3.5 API to create an interactive chatbot experience. This application allows users to:
- Start new conversations
- View chat history
- Mark chats as favorites
- Refresh conversations anytime

## SYSTEM REQUIREMENTS

- **Operating System**: Windows, macOS, or Linux
- **Flutter SDK**: Version 3.0 or later
- **Dart SDK**: Included with Flutter SDK
- **API Key**: OpenAI API key to enable chatbot functionality

## SETUP INSTRUCTIONS

### STEP 1: CLONE THE REPOSITORY

Open a terminal and navigate to the desired directory:

```sh
git clone <repository-url>
cd chat_app_project
```

### STEP 2: INSTALL DEPENDENCIES

Ensure Flutter is installed by running:

```sh
flutter doctor
```

This will confirm that Flutter and Dart SDKs are set up correctly.

Then, install the necessary dependencies:

```sh
flutter pub get
```

### STEP 3: CONFIGURE OPENAI API KEY

Open `lib/contact_page.dart` and locate the `apiKey` variable. Replace the placeholder value with your OpenAI API key:

```dart
final String apiKey = '<your-api-key>';
```

### STEP 4: ADD ASSETS

Ensure the following folder structure in your project directory:

```
assets/
├── chatgpt.jpg
├── nghia.jpg
├── long.jpg
└── thang.jpg
```

Then, reference these assets in the `pubspec.yaml` file:

```yaml
flutter:
  assets:
    - assets/chatgpt.jpg
    - assets/nghia.jpg
    - assets/long.jpg
    - assets/thang.jpg
```

### STEP 5: RUN THE APPLICATION

To run the app on an emulator or connected device:

```sh
flutter run
```

If using an IDE (Android Studio or VSCode), select the desired device before running the command.

## DEMO SCREENSHOTS

### Displaying Chat Messages
Organizes and displays messages between the user and ChatGPT.
![Displaying Chat Messages](https://i.imgur.com/kXJHZ4S.png)

### New Chat
Generate a new chat by clicking on the top right button.
![New Chat](https://i.imgur.com/X2NuxF0.png)

### Saving and Showing Chat History
Keeps track of the conversation, allowing users to view the chat history.
![Saving and Showing Chat History](https://i.imgur.com/Y7WxVF1.png)

## FEATURE TESTING

### TESTING CHAT FUNCTIONALITY

- **Start a New Chat**: On the home screen, type a message to initiate a conversation with the chatbot and confirm the AI’s response.
- **View Chat History**: Access the chat history page from the drawer menu and verify that previous conversations appear correctly.
- **Favorite a Chat**: Mark a conversation as a favorite by tapping the heart icon and check if it appears in the favorites list.
- **Refresh the Chat**: Click the refresh icon on the main screen to start a new conversation.

## NOTES AND ADDITIONAL INFORMATION

- Ensure you have a stable internet connection to receive responses from the OpenAI API.
- Tested on Flutter version 3.0.0, Android 10, and iOS 14 simulators. Compatibility may vary with other OS versions.
- The project uses assets in the `assets/` folder for avatars and logos, so ensure they are correctly referenced.

