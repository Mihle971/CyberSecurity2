 CyberSecurity2 – AI Cybersecurity Chatbot

A Windows desktop chatbot application built with C# and WPF (.NET Framework 4.7.2) that educates users on cybersecurity topics and online safety.



 About The Project

CyberSecurity2 is an interactive AI chatbot designed to help users learn about cybersecurity. It greets users with a voice message, remembers their name, tracks their interests, and responds to questions about topics such as phishing, passwords, firewalls, VPNs, malware, and more. The chatbot also detects the user's emotional state (frustrated, confused, worried, etc.) and responds with empathy.


 Features

 **Voice greeting** – plays an audio welcome when the app launches
  **User memory** – remembers returning users by name using a local text file
  **Keyword-based AI responses** – matches user questions to cybersecurity answers
**Sentiment detection** – recognises emotions like frustration, confusion, and happiness
**Interest tracking** – saves and reminds users of their cybersecurity interests every 3 messages
 **Multi-page UI** – home page, username page, and chat page using WPF grids


 Project Structure


CyberSecurity2/
│
├── MainWindow.xaml          # UI layout – home, username, and chat grids
├── MainWindow.xaml.cs       # Code-behind – event handlers and AI chat logic
├── respond.cs               # Chatbot answer bank and ignore word list
├── user_name.cs             # Username input, memory recall, and welcome messages
├── Voice_greeting.cs        # Plays the greet.wav audio on startup
├── App.xaml                 # WPF application entry point
├── App.xaml.cs              # App startup logic
├── greet.wav                # Audio greeting file
├── logo.png                 # Application logo displayed on home and username pages
└── Properties/              # Assembly info and resources
```

---

 How To Run

Requirements
- Windows 10 or 11
- Visual Studio 2019 or later
- .NET Framework 4.7.2

 Steps
1. Clone or download this repository
2. Open `CyberSecurity2.sln` in Visual Studio
3. Make sure `logo.png` and `greet.wav` are in the project root with **"Copy to Output Directory"** set to **"Copy always"**
4. Press **F5** or click **Start** to run the application

---
 How To Use

1. Launch the app — a voice greeting will play automatically
2. Click **"Proceed"** on the home screen
3. Enter your username and click **"Submit Username"**
4. Type a cybersecurity question in the chat box and click **"Send"**

Example questions you can ask:
- `What is phishing?`
- `How do I create a strong password?`
- `What is a firewall?`
- `Tell me about VPNs`
- `My account was hacked, what do I do?`
- `I am interested in cybersecurity and malware`


Data Files

The app creates two text files in the run directory to store data between sessions:

| File | Purpose |
|------|---------|
| `user_names.txt` | Stores usernames to recognise returning users |
| `interested_topic.txt` | Stores each user's declared interests |


 Built With

- C# — application logic
- WPF (Windows Presentation Foundation) — desktop UI
- .NET Framework 4.7.2
- Visual Studio



 Author

Developed as a cybersecurity awareness chatbot project.
