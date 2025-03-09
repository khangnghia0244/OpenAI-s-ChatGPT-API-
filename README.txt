# 📱 Chat App  

This project is a **Flutter-based chatbot application** using OpenAI's GPT-3.5 API. It allows users to **start new conversations, view chat history, favorite chats, and refresh conversations**.

## ✨ Features  

- **User Management**  
  - Secure registration and login.  
- **Chat Functionality**  
  - AI-powered chatbot interaction.  
- **Chat History**  
  - View and manage past conversations.  
- **Favorites**  
  - Mark important chats for easy access.  

## ⚙️ System Requirements  
- **OS**: Windows, macOS, or Linux  
- **Flutter SDK**: Version 3.0 or later  
- **Dart SDK**: Included with Flutter  
- **API Key**: OpenAI API key  

## 🚀 Setup Instructions  

### 1️⃣ Clone the Repository  
```bash
git clone <repository-url>
cd chat_app_project
```

### 2️⃣ Install Dependencies  
```bash
flutter doctor  # Check Flutter installation
flutter pub get  # Install dependencies
```

### 3️⃣ Configure OpenAI API Key  
Open `lib/contact_page.dart` and replace `apiKey` with your OpenAI API key:  
```dart
final String apiKey = 'your_api_key_here';
```

### 4️⃣ Add Assets  
Ensure the `assets/` folder has required images:  
```plaintext
assets/
├── chatgpt.jpg
├── nghia.jpg
├── long.jpg
└── thang.jpg
```

Update `pubspec.yaml`:  
```yaml
flutter:
  assets:
    - assets/chatgpt.jpg
    - assets/nghia.jpg
    - assets/long.jpg
    - assets/thang.jpg
```

### 5️⃣ Run the Application  
```bash
flutter run
```

## 🛠 Feature Testing  
- ✅ **Start a Chat**: Type a message to begin a conversation.  
- ✅ **View Chat History**: Access past conversations via the menu.  
- ✅ **Mark Favorite**: Tap the heart icon to save a chat.  
- ✅ **Refresh**: Restart a new conversation anytime.  
