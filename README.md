<div align="center">

# 🤖 Scarlett — Virtual Assistant

### Voice-controlled AI assistant in Python

![python](https://img.shields.io/badge/Python-3.9+-3776AB?logo=python&logoColor=white)
![speech](https://img.shields.io/badge/Speech-Recognition-blue)
![last commit](https://img.shields.io/github/last-commit/virinchisai/Scarlett-Virtual-Assistant)
![stars](https://img.shields.io/github/stars/virinchisai/Scarlett-Virtual-Assistant?style=social)

</div>

Scarlett is a voice-controlled **virtual assistant** that takes natural-language
spoken commands and responds via speech. Built in Python with speech-recognition
and text-to-speech libraries.

## 📰 Publication

> **Scarlett: Virtual Assistant and Browlett Browser**

## 🏗️ How it works

```mermaid
flowchart LR
    Mic[🎙️ Microphone] --> SR[Speech<br/>Recognition]
    SR --> Cmd[Command<br/>Parser]
    Cmd --> Web[🌐 Web Search]
    Cmd --> App[💻 App Launch]
    Cmd --> Sys[⚙️ System Control]
    Cmd --> Time[⏰ Time / Weather]
    Web --> TTS[Text-to-Speech]
    App --> TTS
    Sys --> TTS
    Time --> TTS
    TTS --> Speaker[🔊 Speaker]
```

## ✨ Capabilities

- Web search and read top results aloud
- Launch applications
- Tell time, date, weather
- Open websites
- System control (volume, shutdown, etc.)
- Conversational responses

## 🚀 Quick start

```bash
pip install SpeechRecognition pyttsx3 pyaudio wikipedia
python scarlett2.py
```

Say "Hello Scarlett" to wake it.

### Email configuration

Email sending is optional. Configure SMTP credentials in your shell before
starting Scarlett. For Gmail, use an app password instead of your account
password.

```bash
export SCARLETT_SMTP_USERNAME="your-email@gmail.com"
export SCARLETT_SMTP_PASSWORD="your-app-password"
python scarlett2.py
```

Optional `SCARLETT_SMTP_HOST` and `SCARLETT_SMTP_PORT` variables default to
`smtp.gmail.com` and `587`. Never commit credentials or a populated `.env`
file.

## 📜 License
MIT
