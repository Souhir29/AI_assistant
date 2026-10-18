# 🤖 AI Math Assistant — Hand Gesture Calculator

> Draw math expressions in the air with your hand and let **Google Gemini AI** solve them in real time!

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-1.x-red?logo=streamlit)
![Google Gemini](https://img.shields.io/badge/Google-Gemini_AI-orange?logo=google)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green?logo=opencv)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

## ✨ Features

- 🖐️ **Real-time hand tracking** using your webcam (MediaPipe + cvzone)
- ✏️ **Draw math expressions** in the air with your index finger
- 🧹 **Erase the canvas** by raising your thumb
- 🤖 **AI-powered solving** with Google Gemini — raise 4 fingers to send the expression
- 🖥️ **Clean web UI** built with Streamlit

---

## 🖐️ Gesture Controls

| Gesture | Action |
|---|---|
| ☝️ Index finger up | Draw on canvas |
| 👍 Thumb up only | Clear canvas & reset |
| 🖐️ 4 fingers up (no pinky) | Send to Gemini AI for solving |

---

## 🚀 Getting Started

### 1. Prerequisites

- Python **3.8+**
- A working **webcam**
- A **Google Gemini API key** → [Get one here](https://aistudio.google.com/app/apikey)

### 2. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/AI_assistant.git
cd AI_assistant
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Set up your API key

Create a `.env` file at the root of the project:

```env
GOOGLE_API_KEY=your_google_gemini_api_key_here
```

> ⚠️ **Never commit your `.env` file!** It is already listed in `.gitignore`.

### 5. Run the app

```bash
streamlit run main.py
```

The app will open automatically in your browser at `http://localhost:8501`.

---

## 📁 Project Structure

```
AI_assistant/
├── main.py            # Main application logic
├── requirements.txt   # Python dependencies
├── .env               # Your API key (NOT committed to git)
├── .gitignore         # Files to ignore in git
└── README.md          # This file
```

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| [OpenCV](https://opencv.org/) | Webcam capture & image processing |
| [cvzone](https://github.com/cvzone/cvzone) | Hand tracking helper |
| [MediaPipe](https://mediapipe.dev/) | Hand landmark detection |
| [Google Gemini](https://ai.google.dev/) | AI math expression solving |
| [Streamlit](https://streamlit.io/) | Web UI framework |
| [Pillow](https://python-pillow.org/) | Image conversion |
| [NumPy](https://numpy.org/) | Canvas array manipulation |

---

## 📝 License

This project is licensed under the **MIT License** — feel free to use, modify, and distribute it.

---

## 🙌 Acknowledgements

- [cvzone by CVZone](https://github.com/cvzone/cvzone) for the amazing hand tracking module
- [Google AI Studio](https://aistudio.google.com/) for the Gemini API
