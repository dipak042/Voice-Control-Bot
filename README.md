# 🤖 Pinky Bot — AI Voice-Controlled Assistant

**Pinky Bot** is an interactive, browser-based **AI voice assistant** built with React. It combines **speech recognition, Google Gemini AI, text-to-speech, and browser actions** to create a conversational virtual robot assistant.

The application can listen to voice commands, understand user requests, respond using Gemini, speak responses aloud, and perform actions such as Google searches, YouTube searches, and opening websites.

---

## ✨ Features

### 🎙️ Voice Recognition

* Uses the browser's Web Speech API
* Converts spoken commands into text
* Supports `en-IN` speech recognition
* Displays the recognized transcript
* Listening state is shown through the robot interface

### 🧠 Gemini AI Integration

Pinky Bot uses the **Google Gemini API** to generate conversational responses.

The assistant is configured with a custom personality prompt that makes responses:

* Short
* Friendly
* Fun
* High-energy
* Conversational

### 🔊 Text-to-Speech

The assistant can speak its responses using the browser's `SpeechSynthesis` API.

It also:

* Selects an available voice
* Adjusts speech pitch
* Controls speech rate
* Shows a speaking state in the UI

### 🌐 Voice-Controlled Web Actions

Pinky Bot can perform browser actions from voice commands.

Examples:

```text
"Search for artificial intelligence"
```

→ Opens a Google search.

```text
"Play relaxing music on YouTube"
```

→ Opens YouTube search results.

```text
"Open instagram.com"
```

→ Opens the requested website.

### 😂 Local Commands

Some commands are handled locally without calling Gemini.

For example:

```text
"Tell me a joke"
```

The application selects a random predefined robot joke.

### 🕐 Time Command

The assistant can provide the current local time using JavaScript's `Date` API.

### 🤖 Animated Robot Interface

The application includes an interactive robot visualization with:

* Animated blinking eyes
* Eye movement following the mouse
* Animated antenna
* Speaking animation
* Listening animation
* Dynamic heart indicator
* Robot mood states
* Parallax background effects

### ⚡ Quick Actions

The interface provides quick buttons for:

* 😂 Tell Joke
* 🔍 Search Cats
* 📸 Open Instagram

---

## 🛠️ Tech Stack

| Technology              | Purpose                    |
| ----------------------- | -------------------------- |
| **React**               | Front-end application      |
| **JavaScript**          | Application logic          |
| **Google Gemini API**   | AI responses               |
| **Web Speech API**      | Speech recognition         |
| **SpeechSynthesis API** | Text-to-speech             |
| **Lucide React**        | UI icons                   |
| **SVG**                 | Custom robot visualization |
| **Tailwind CSS**        | UI styling                 |

---

## 🧠 How It Works

```text
                  🎙️ User Voice
                       │
                       ▼
             ┌──────────────────┐
             │ Speech Recognition│
             └────────┬─────────┘
                      │
                      ▼
              Command Processing
                      │
          ┌───────────┼───────────┐
          │           │           │
          ▼           ▼           ▼
       Search       YouTube      Local
       /Open         Action      Command
          │           │           │
          └───────────┼───────────┘
                      │
                 Other Queries
                      │
                      ▼
              ┌───────────────┐
              │ Gemini AI API │
              └───────┬───────┘
                      │
                      ▼
               AI Response
                      │
              ┌───────┴────────┐
              │                │
              ▼                ▼
        Display Text      Text-to-Speech
                              │
                              ▼
                       🔊 Voice Response
```

---

## 📂 Project Structure

```text
Voice-Control-Bot/
│
├── src/
│   ├── App.jsx
│   ├── ...
│
├── public/
│   └── ...
│
├── package.json
├── README.md
└── ...
```

> Update the structure if your repository uses different filenames or folders.

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/dipak042/Voice-Control-Bot.git
```

### 2. Navigate to the project

```bash
cd Voice-Control-Bot
```

### 3. Install dependencies

```bash
npm install
```

### 4. Configure Gemini API

The application uses the Google Gemini API.

Create an environment variable for your Gemini API key instead of committing the key to GitHub.

Example:

```env
VITE_GEMINI_API_KEY=your_api_key_here
```

Then configure your application to read the key from the environment.

> ⚠️ Never commit API keys or other secrets to a public repository.

### 5. Start the development server

```bash
npm run dev
```

Open the local development URL shown by Vite in your browser.

---

## 🎤 Example Voice Commands

### AI Conversation

```text
"Tell me something interesting"
```

### Google Search

```text
"Search for Python tutorials"
```

### YouTube

```text
"Play coding music on YouTube"
```

### Website

```text
"Open github.com"
```

### Local Commands

```text
"Tell me a joke"
```

```text
"What is the time?"
```

---

## 🔐 API & Privacy

This project requires access to the Gemini API for AI-generated responses.

The application also uses browser speech-recognition and speech-synthesis capabilities.

Because voice processing depends on browser APIs and configuration, behavior may vary between browsers.

**Never expose your Gemini API key in publicly accessible source code.**

---

## 🎨 User Interface

Pinky Bot features a custom robot interface with:

* Pink/rose visual theme
* Animated robot character
* Interactive eyes
* Voice status indicator
* Dynamic robot moods
* Speaking animation
* Large microphone control
* Quick command buttons
* Responsive card-based interface

The robot reacts visually to states such as:

```text
IDLE
  ↓
LISTENING
  ↓
THINKING
  ↓
SPEAKING
  ↓
IDLE
```

---

## 🎯 Project Objectives

The project was developed to explore the integration of:

* Artificial Intelligence
* Voice interfaces
* Browser APIs
* React development
* Generative AI
* Text-to-speech technology
* Natural language interaction
* Interactive UI/UX

---

## 📚 Learning Outcomes

Through this project, I gained practical experience with:

* React state management
* React hooks such as `useState`, `useEffect`, and `useRef`
* REST API integration
* Gemini API integration
* Browser speech recognition
* Browser speech synthesis
* Asynchronous JavaScript
* Event handling
* Dynamic UI states
* SVG-based graphics
* Responsive interface design

---

## 🚀 Future Improvements

* [ ] Add persistent conversation memory
* [ ] Add multiple AI personalities
* [ ] Add Hindi/Bengali voice support
* [ ] Add weather and news commands
* [ ] Add music controls
* [ ] Add application shortcuts
* [ ] Add authentication
* [ ] Improve error handling
* [ ] Add mobile optimization
* [ ] Add configurable AI model settings
* [ ] Add command history
* [ ] Add more browser automation features

---

## ⚠️ Current Limitations

* Voice recognition depends on browser support.
* Gemini responses require API access.
* Browser permissions may be required for microphone access.
* Some voice/browser features can behave differently across browsers.
* Web actions are limited to the commands implemented in the application.

---

## 👨‍💻 Author

**Dipak Hrishi Das**

B.Tech — Electronics & Communication Engineering

Interested in:

* Artificial Intelligence
* Software Development
* Full-Stack Development
* IoT
* Embedded Systems

### Connect

* GitHub: [@dipak042](https://github.com/dipak042)
* LinkedIn: [Dipak Hrishi Das](https://www.linkedin.com/in/dipak-hrishi-das)

---

## ⭐ Support

If you like this project, consider giving the repository a ⭐ on GitHub.
