# 💻 CompTIA A+ Core 2 (220-1202) Training Interface

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This repository hosts a self-contained, interactive, front-end web application designed to help users study and prepare for the **CompTIA A+ Core 2 (220-1202)** certification exam. It features multiple practice modules, including practice tests, mixed review drills, a troubleshooting simulator, and a self-contained AI study bot.

## 🚀 Key Features

* **Multiple Practice Exams:** Access consolidated question sets from Professor Messer, Dion Training, and other supplementary sources.
* **Mixed Review Drills:** Generate randomized quizzes of custom length from the entire combined question pool.
* **Interactive Chatbot (Cooper AI):** A self-contained, client-side AI assistant to answer study questions, direct users to relevant modules, and run an interactive troubleshooting Q&A game.
* **Aesthetic UI:** A clean, responsive, glassmorphic interface designed for focused study.
* **Study Resources:** Direct links to official exam objectives, glossary terms, and essential command-line references.
* **Dynamic Sidebar:** Displays local time and is configured for optional real-time weather integration (requires a private API key).

---

## ⚠️ Intellectual Property Disclaimer

**This application is designed solely for personal study and non-commercial educational use.**

I do not claim ownership of the practice exam content, including the quiz questions sourced from Professor Messer, Dion Training, or ExamCompass. All rights and intellectual property belong to the respective content creators and owners. This project utilizes publicly available or student-generated question pools combined into a single interface for user convenience.

---

## 🛠️ Installation and Setup

Since this is a purely front-end application built with HTML, CSS, and JavaScript, no complex installation or server configuration is required.

### Local Setup (Easiest Method)

1.  **Clone the Repository:**
    ```bash
    git clone [Your Repository URL Here]
    ```
2.  **Navigate to the Directory:**
    ```bash
    cd [repository-name]
    ```
3.  **Open in Browser:** Simply double-click the `index.html` file, or open it in your browser (e.g., `file:///path/to/repo/index.html`).

### Enabling Real-Time Weather

The sidebar includes a weather widget, but it requires a free API key to function:

1.  **Get a Key:** Sign up for a free account at **OpenWeatherMap** to obtain an API Key (APPID).
2.  **Edit `index.html`:** Open `index.html` and find the following lines in the main `<script>` block:
    ```javascript
    const OPENWEATHER_API_KEY = ''; // <-- PASTE YOUR OPENWEATHERMAP API KEY HERE
    const CITY_NAME = 'New York'; // <-- SET YOUR CITY HERE
    ```
3.  **Update:** Paste your key and change `CITY_NAME` to your desired location.

---

## 🤖 Using Cooper AI (The Study Bot)

The chatbot runs entirely in your browser and does not require an internet connection for basic interaction or the Q&A game.

1.  Click the **red circular button** in the bottom-right corner to open the chat widget.
2.  **Conversation Mode:** Ask general questions (e.g., "Where are the video resources?" or "What is BitLocker?").
3.  **Q&A Game Mode:** Type **`Start Quiz`** to begin an interactive flashcard session on the A+ troubleshooting model.
    * During the game, you can type **`Hint`** for a clue or **`Give Answer`** to skip the current step.

---

## 📜 Repository Structure

| File | Description |
| :--- | :--- |
| `index.html` | The main interface page. Contains the site layout, all styling (CSS), and the core JavaScript logic (AI, clock, navigation). |
| `quiz-a.html` | Practice Test A module (Professor Messer). |
| `dion.html` | Practice Test module (Dion Training). |
| `quiz-random.html` | The dynamic quiz generator which pulls and randomizes questions from all major test files. |
| `tips.js` | Contains the data array for the "Core 2 Spotlight" tip section. |
| `commands.html` | (Placeholder/Link) Command-line reference sheet. |
| `glossary.html` | (Placeholder/Link) Key term definitions. |
| `objectives.html` | (Placeholder/Link) Exam objective breakdown. |

---

## 🤝 Contributing

This project is primarily a study tool, but suggestions for improvements to the interface, new features, or identified errors in the quiz code are welcome.

Please submit bug reports or feature requests using the GitHub Issues tracker.

---

## ⚖️ License

This project is licensed under the MIT License - see the `LICENSE` file for details.
