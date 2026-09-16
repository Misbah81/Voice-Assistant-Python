# 🎙️ Voice Assistant Python

> **A Windows-based Python Voice Assistant that combines Speech Recognition, Text-to-Speech, AI-assisted responses, browser automation, file operations, document generation, QR-code creation, and voice-controlled programming tasks.**

[![Python](https://img.shields.io/badge/Python-3.12+-3776AB?style=for-the-badge\&logo=python\&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge\&logo=jupyter\&logoColor=white)](https://jupyter.org/)
[![Speech Recognition](https://img.shields.io/badge/Speech-Recognition-4CAF50?style=for-the-badge)](#)
[![AI](https://img.shields.io/badge/AI-Experiments-8E44AD?style=for-the-badge)](#)
[![Platform](https://img.shields.io/badge/Platform-Windows-0078D4?style=for-the-badge\&logo=windows\&logoColor=white)](#)

---

## 📌 Overview

**Voice Assistant Python** is a Python-based voice automation and AI experimentation project developed as a collection of practical implementations inside a Jupyter Notebook.

The project allows voice input to be converted into commands and used for tasks such as:

* 🎤 Speech recognition
* 🔊 Text-to-speech responses
* 🌐 Google and YouTube searching
* 🌍 Browser automation
* 📝 Voice-controlled note creation
* 📁 Folder and file creation
* 💻 Python file generation and execution
* 🧑‍💻 Visual Studio Code automation
* 📄 Word document generation
* 🔲 QR-code generation
* 🤖 AI-assisted text responses
* 🖼️ AI image-generation experiments
* 💬 ChatterBot and spaCy experiments

Rather than being a single fixed chatbot application, the notebook contains **multiple independently developed and tested voice-assistant modules and automation experiments**.

---

# ✨ Key Highlights

### 🎤 Voice Interaction

Convert spoken commands into executable actions using speech recognition.

### 🔊 Text-to-Speech

The assistant can respond through synthesized speech instead of relying only on text output.

### 🌐 Browser Automation

Voice commands can be used to interact with Google Chrome and perform searches.

### 💻 Voice-Controlled Programming

The project experiments with creating Python files, writing code into them, running them, and controlling Visual Studio Code through voice commands.

### 🤖 AI Integration

AI-assisted experiments explore different workflows such as:

```text
Speech → Text → AI → Text
```

```text
Speech → Text → AI → Speech
```

and:

```text
Speech → Text → AI → Image
```

### 📄 Productivity Automation

The assistant can also be used for practical tasks such as:

* Creating notes
* Creating folders
* Generating Python files
* Creating Word documents
* Generating QR codes

---

# 🧩 Features

## 🎙️ Speech & Voice Features

* Speech-to-text using `SpeechRecognition`
* Text-to-speech using `pyttsx3`
* Voice wake-word interaction
* Wake word: `hello`
* Voice-controlled commands
* Voice-based note creation
* Spoken command processing

---

## 🌐 Browser Automation

The notebook includes experiments for:

* Opening Google Chrome
* Minimizing the browser
* Searching Google using voice commands
* Searching YouTube using voice commands
* Browser interaction through automation
* YouTube interface detection using OpenCV template matching

Example commands:

```text
search from google
search from youtube
minimise the browser
```

---

## 💻 Voice-Controlled Development

The assistant includes automation experiments for programming tasks.

It can be used to:

```text
Open VS Code
       ↓
Create a Python file
       ↓
Write code
       ↓
Run the Python file
       ↓
Close VS Code
```

Example commands:

```text
open vs code
make python file
write code
run the code
close vs code
```

---

## 📝 File & Document Automation

The project includes voice-based automation for:

* Creating folders
* Creating files
* Writing content into files
* Creating Python source files
* Generating Word documents
* Saving notes to a selected directory

---

## 🔲 QR Code Generation

The project includes QR-code generation using Python.

Basic workflow:

```text
Input Data
    ↓
Python QR Generator
    ↓
QR Code
    ↓
Image File
```

Technology used:

```text
qrcode + Pillow
```

---

# 🤖 AI Experiments

The notebook also contains AI-assisted experiments using `g4f`.

### Text → Text

```text
User Input
    ↓
AI Model / Provider
    ↓
Text Response
```

### Speech → Text → AI

```text
Voice Input
    ↓
Speech Recognition
    ↓
Text
    ↓
AI
    ↓
Response
```

### Speech → Text → AI → Speech

```text
Voice Input
    ↓
Speech-to-Text
    ↓
AI Response
    ↓
Text-to-Speech
    ↓
Voice Output
```

### Speech → Text → Image

The notebook also contains experiments involving AI-assisted image generation based on user input.

> **Note:** AI-related functionality depends on third-party providers and the installed `g4f` version. Provider availability and APIs can change independently of this repository.

---

# 🧠 Technologies & Libraries

| Technology           | Purpose                              |
| -------------------- | ------------------------------------ |
| 🐍 Python            | Core programming language            |
| 📓 Jupyter Notebook  | Development and experimentation      |
| 🎤 SpeechRecognition | Speech-to-text                       |
| 🔊 pyttsx3           | Text-to-speech                       |
| 🗣️ gTTS             | Text-to-speech experiments           |
| 🤖 g4f               | AI-assisted experiments              |
| 🌐 PyAutoGUI         | GUI automation                       |
| 🪟 PyGetWindow       | Window management                    |
| 👁️ OpenCV           | Image processing / template matching |
| 🔢 NumPy             | Numerical operations                 |
| 📱 qrcode            | QR-code generation                   |
| 🖼️ Pillow           | Image handling                       |
| 📄 python-docx       | Word document generation             |
| 💬 ChatterBot        | Conversational AI experiments        |
| 🧠 spaCy             | NLP experimentation                  |
| 📚 Wikipedia         | Information retrieval                |

---

# 🏗️ Project Structure

```text
Voice-Assistant-Python/
│
├── updated_python_project.ipynb
│
├── README.md
│
├── requirements.txt
│
└── .gitignore
```

### Main Notebook

```text
updated_python_project.ipynb
```

The notebook contains the complete collection of voice-assistant implementations and experiments.

---

# 🔄 Overall Workflow

The project follows several different workflows depending on the selected notebook section.

### Voice Command Workflow

```text
┌─────────────────┐
│   User Speaks   │
└────────┬────────┘
         ↓
┌─────────────────┐
│ SpeechRecognition│
└────────┬────────┘
         ↓
┌─────────────────┐
│ Convert to Text │
└────────┬────────┘
         ↓
┌─────────────────┐
│ Command Matching│
└────────┬────────┘
         ↓
┌─────────────────────────────┐
│ Execute Requested Operation │
└──────────────┬──────────────┘
               ↓
      ┌────────┴────────┐
      ↓                 ↓
  Automation        AI Response
      ↓                 ↓
   Result          Text / Speech
```

---

# 🖥️ System Requirements

### Recommended Environment

* Windows operating system
* Python 3.12+
* Microphone
* Speakers or headphones
* Internet connection
* Google Chrome for browser automation
* Visual Studio Code for VS Code automation
* Microsoft Word for Word-document functionality

The notebook metadata was created using:

```text
Python 3.12.4
```

---

# ⚙️ Installation

## 1️⃣ Clone the Repository

Open **Command Prompt**, **PowerShell**, or **Anaconda Prompt**:

```bash
git clone https://github.com/Misbah81/Voice-Assistant-Python.git
```

Move into the project directory:

```bash
cd Voice-Assistant-Python
```

---

## 2️⃣ Create a Virtual Environment

### Using Python

```bash
python -m venv venv
```

Activate it:

```bash
venv\Scripts\activate
```

### OR Using Anaconda

```bash
conda create -n voice_assistant python=3.12
```

Activate:

```bash
conda activate voice_assistant
```

---

## 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

Install Jupyter Notebook:

```bash
pip install notebook
```

---

# ▶️ Running the Project

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
updated_python_project.ipynb
```

Then execute the required notebook sections.

> **Important:** The notebook contains multiple independent experiments. It is not intended to be executed as one single linear application from the first cell to the last.

---

# 🎙️ Example Voice Commands

Some commands implemented in the notebook include:

```text
hello
```

```text
write a note
```

```text
search from google
```

```text
search from youtube
```

```text
minimise the browser
```

```text
open vs code
```

```text
make python file
```

```text
write code
```

```text
run the code
```

```text
close vs code
```

```text
generate qr code
```

```text
create document
```

The exact supported commands depend on the individual notebook section being executed.

---

# 🪟 Windows Configuration

Some features interact directly with Windows applications and therefore may require local configuration.

## Visual Studio Code Path

One automation section uses:

```text
C:\Program Files\Microsoft VS Code\Code.exe
```

If VS Code is installed in another location, update the path in the corresponding notebook cell.

---

## 🎤 Microphone

Speech recognition uses:

```python
sr.Microphone()
```

Make sure:

* A microphone is connected
* Windows microphone permission is enabled
* The correct input device is selected
* No other application is blocking the microphone

---

## 🖼️ OpenCV Template

The YouTube template-matching experiment uses:

```text
template6.png
```

The image must be available at the path used by the corresponding notebook cell.

For better portability, a relative path can be used:

```python
template6 = cv2.imread("template6.png", 0)
```

instead of a machine-specific absolute path.

---

# 📦 Dependencies

The main dependencies are listed in:

```text
requirements.txt
```

Install everything with:

```bash
pip install -r requirements.txt
```

If a particular package fails to install, install it separately according to your Python and operating-system configuration.

---

# 🛠️ Troubleshooting

## `ModuleNotFoundError`

Install the missing package:

```bash
pip install PACKAGE_NAME
```

Or reinstall the project dependencies:

```bash
pip install -r requirements.txt
```

---

## 🎤 Microphone Not Working

Check:

* Windows microphone permissions
* Default recording device
* Physical microphone connection
* PyAudio installation
* Whether another application is using the microphone

---

## 🗣️ Speech Recognition Not Understanding Commands

Make sure you:

1. Have an active internet connection.
2. Wait until the program starts listening.
3. Speak clearly.
4. Use a command supported by the current notebook section.

The speech-recognition sections use an online recognition service, so internet connectivity is required.

---

## 🌐 Browser Automation Not Working

Check:

* Google Chrome is installed.
* Chrome is open when required.
* The correct browser window is available.
* Windows allows the automation.
* The command matches the implemented keywords.

---

## 👁️ OpenCV Template Matching Error

Check:

* `template6.png` exists.
* The image path is correct.
* The template image is readable.
* The screenshot is large enough for the selected template.

---

# 🔐 Security & Privacy

This project performs operations involving:

* Microphone input
* Browser automation
* Local files
* Local applications
* AI/online services


# ⚠️ Third-Party Services

Some project features depend on external software or services.

Examples include:

* Speech-recognition services
* AI providers accessed through `g4f`
* Google
* YouTube
* Chrome
* Visual Studio Code

These services can change independently of this project.

Therefore, a feature that worked with one version of a library/provider may require changes after an external update.

---

# 📸 Screenshots & Demo

<img width="290" height="290" alt="ali_qrcode-checkpoint" src="https://github.com/user-attachments/assets/f7eac603-40b8-4f09-ac64-b63affebb824" />
<img width="1280" height="720" alt="sirsyed-checkpoint" src="https://github.com/user-attachments/assets/4ea62543-1963-4531-9088-ecfb23336ea8" />
<img width="290" height="290" alt="misbah_qrcode-checkpoint" src="https://github.com/user-attachments/assets/72b255f5-9858-4005-a48f-a35d3bfa0d21" />

```

# 🚀 Possible Future Improvements

The current project can be extended with:

* 🔐 User authentication
* 🧠 Better command classification
* 🗂️ Modular Python architecture instead of a single notebook
* 🎯 Intent detection
* 💾 Conversation history
* 🧠 Local LLM integration
* 🔎 RAG-based knowledge retrieval
* 🖥️ Desktop GUI
* 🌐 Web dashboard
* 📱 Mobile control interface
* 🔌 IoT device control
* ⚡ Background voice activation
* 🗣️ Improved multilingual speech recognition

---

# 🎓 Project Purpose

This project was developed as a practical exploration of how Python can combine:

```text
Speech Recognition
       +
Text-to-Speech
       +
AI
       +
Automation
       +
Computer Vision
       +
File Operations
       +
Document Generation
```

It demonstrates the integration of multiple Python libraries into practical voice-controlled workflows.

---

# 📚 Learning Areas Covered

Through this project, the following concepts are explored:

* Python programming
* Functions and modules
* Exception handling
* Speech processing
* Text-to-speech
* Natural language interaction
* GUI automation
* Browser automation
* File handling
* Image processing
* AI API/provider integration
* Document generation
* QR-code generation
* NLP experimentation
* Jupyter Notebook development

---

# 👩‍💻 Author

## Misbah Rafique

**Computer Engineering Student**

Sir Syed University of Engineering & Technology, Karachi

### GitHub

**[@Misbah81](https://github.com/Misbah81)**

---

# ⭐ Support the Project

If you find this project useful for learning Python, automation, speech processing, or AI integration:

⭐ **Star the repository**

🍴 **Fork the repository**

📚 **Explore the notebook**

💡 **Build your own extensions**


# ⚠️ Disclaimer

This is a **personal educational and experimentation project**.

The repository contains multiple independently developed notebook sections. Some features depend on Windows applications, local system configuration, internet connectivity, third-party libraries, and external service/provider availability.

The project should therefore be considered a **learning and experimentation project rather than a production-ready voice assistant**.
