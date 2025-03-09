🚀 SETUP INSTRUCTIONS
1️⃣ CLONE THE REPOSITORY
Open a terminal and navigate to your desired directory. Then, run:

bash
Copy
Edit
git clone <repository-url>
cd chat_app_project
2️⃣ INSTALL DEPENDENCIES
Ensure Flutter is installed:

bash
Copy
Edit
flutter doctor
Then, install the required dependencies:

bash
Copy
Edit
flutter pub get
3️⃣ CONFIGURE OPENAI API KEY
Open lib/contact_page.dart and locate the apiKey variable. Replace the placeholder with your OpenAI API key:

dart
Copy
Edit
final String apiKey = 'your-api-key-here';
4️⃣ ADD ASSETS
Ensure the assets/ folder contains the necessary images (e.g., profile pictures and logos). The directory should look like this:

plaintext
Copy
Edit
assets/
├── chatgpt.jpg
├── nghia.jpg
├── long.jpg
└── thang.jpg
Then, add them to pubspec.yaml:

yaml
Copy
Edit
flutter:
  assets:
    - assets/chatgpt.jpg
    - assets/nghia.jpg
    - assets/long.jpg
    - assets/thang.jpg
5️⃣ RUN THE APPLICATION
To run the app on an emulator or connected device, use:

bash
Copy
Edit
flutter run
If you're using an IDE like Android Studio or VSCode, select your device before running.

✅ FEATURE TESTING
START A NEW CHAT: Type a message to start chatting with the AI.
VIEW CHAT HISTORY: Check past conversations in the chat history menu.
FAVORITE A CHAT: Mark a chat as favorite by tapping the heart icon.
REFRESH THE CHAT: Click the refresh icon to start a new conversation.
ℹ️ NOTES AND ADDITIONAL INFORMATION
A stable internet connection is required for chatbot responses.
Tested on Flutter 3.0.0, Android 10, and iOS 14 simulators. Compatibility may vary.
Ensure that the assets/ folder is correctly referenced in pubspec.yaml.
