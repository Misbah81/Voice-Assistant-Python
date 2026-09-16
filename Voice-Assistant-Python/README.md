# Voice Assistant Python Project

A Windows-focused Python voice assistant and experimentation project built around speech recognition, text-to-speech, browser automation, file operations, QR-code generation, document creation, and AI-assisted text/speech experiments.

The main implementation is provided as a Jupyter Notebook: `updated_python_project.ipynb`.

## Features

The notebook contains implementations/experiments for:

- Voice wake-word interaction using the word `hello`
- Text-to-speech responses with `pyttsx3`
- Speech-to-text using `SpeechRecognition`
- Voice-controlled note creation
- Saving notes into a selected directory
- Opening and controlling Google Chrome
- Minimizing the Chrome browser
- Searching Google using voice commands
- Searching YouTube using voice commands
- Attempting YouTube ad-button detection with OpenCV/template matching
- Opening Visual Studio Code
- Creating folders through voice commands
- Creating Python files through voice commands
- Writing code into Python files through voice input
- Running Python files through the assistant
- Closing Visual Studio Code
- QR-code generation
- Creating Word documents from spoken content
- Text-to-text AI experiments using `g4f`
- Speech-to-text + AI response experiments
- Speech-to-speech experiments using AI-generated responses
- Speech-to-image experiments
- ChatterBot + spaCy experimentation

## Project Structure

```text
Voice-Assistant-Python/
│
├── updated_python_project.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Technologies Used

- Python
- Jupyter Notebook
- SpeechRecognition
- PyAudio
- pyttsx3
- g4f
- gTTS
- OpenCV
- NumPy
- PyAutoGUI
- PyGetWindow
- Wikipedia API/library
- qrcode
- Pillow
- python-docx
- ChatterBot
- spaCy

## Requirements

Recommended:

- Windows
- Python 3.12+
- Microphone
- Speakers/headphones
- Internet connection for speech recognition and the online AI/search experiments
- Google Chrome for browser-related commands
- Microsoft Word for the Word-document workflow
- Visual Studio Code for VS Code automation

The notebook metadata was created with Python 3.12.4.

## Installation

### 1. Clone the repository

Open Command Prompt, PowerShell, or Anaconda Prompt:

```bash
git clone https://github.com/YOUR-USERNAME/Voice-Assistant-Python.git
cd Voice-Assistant-Python
```

Replace `YOUR-USERNAME` with your GitHub username.

### 2. Create a virtual environment

Using Python:

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

Or with Anaconda:

```bash
conda create -n voice_assistant python=3.12
conda activate voice_assistant
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

If PyAudio gives an installation error on Windows, install it separately using a compatible wheel/package for your Python version.

### 4. Install Jupyter

```bash
pip install notebook
```

Then start Jupyter:

```bash
jupyter notebook
```

Open:

```text
updated_python_project.ipynb
```

## How to Run

Because the notebook contains multiple independent experiments, run the section you want rather than treating every cell as one single application.

For the voice-controlled sections:

1. Connect a working microphone.
2. Make sure Windows has microphone permission enabled.
3. Run the required notebook cell.
4. Say the wake word:

```text
hello
```

5. Then speak the command supported by that section.

Examples used in the notebook include:

```text
hello
write a note
search from google
search from youtube
minimise the browser
open vs code
make python file
write code
run the code
close vs code
generate qr code
create document
```

## Important Windows Notes

Some parts of this project interact directly with Windows applications.

### Visual Studio Code path

One VS Code automation section uses:

```text
C:\Program Files\Microsoft VS Code\Code.exe
```

If VS Code is installed somewhere else, update that path in the relevant notebook cell.

### YouTube template image

The YouTube ad-skipping experiment uses an OpenCV template image named:

```text
template6.png
```

Place the image in the project directory and update the notebook path if necessary.

A portable version should use a relative path such as:

```python
template6 = cv2.imread("template6.png", 0)
```

instead of a machine-specific absolute path.

### Microphone

The speech-recognition functions use:

```python
sr.Microphone()
```

Make sure a microphone is available and selected correctly in Windows.

## AI / g4f Experiments

Some notebook sections use the `g4f` package for AI-related experiments.

These experiments include:

- Text → Text
- Speech → Text → AI response
- Speech → Text → AI response → Speech
- Speech → Text → Image-generation experiments

These integrations depend on third-party providers and may change independently of this repository. A working setup can therefore depend on the installed `g4f` version and provider availability.

No private API key should be committed to this repository.

## Security

Do not commit:

- API keys
- Passwords
- Authentication tokens
- Personal files
- Private recordings
- Personal documents
- Provider credentials

If you later add credentials, store them in environment variables or a local `.env` file and keep `.env` in `.gitignore`.

## Troubleshooting

### `ModuleNotFoundError`

Install the missing package:

```bash
pip install PACKAGE_NAME
```

or reinstall all dependencies:

```bash
pip install -r requirements.txt
```

### Microphone not working

Check:

- Windows microphone permission
- Default recording device
- Microphone connection
- PyAudio installation
- Whether another application is using the microphone

### Speech recognition does not understand the command

Speak clearly and wait for the notebook to print:

```text
Listening...
```

Speech recognition in the notebook uses Google's recognition service, so an internet connection is required for those calls.

### Browser automation does not work

Make sure:

- Google Chrome is open when required
- The correct window is visible
- Windows permissions allow the automation
- The command matches the keywords implemented in that notebook section

### OpenCV template matching error

The YouTube ad-skipping section requires a valid `template6.png` image and a screenshot that is large enough for the template. Check the image path and template dimensions.

## GitHub Upload

After testing the repository locally:

```bash
git init
git add .
git commit -m "Initial commit - Python Voice Assistant"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/Voice-Assistant-Python.git
git push -u origin main
```

Replace `YOUR-USERNAME` with your GitHub username.

## Author

**Misbah Rafique**

Computer Engineering Student

## Disclaimer

This repository is a personal educational project containing multiple Python experiments developed and tested as separate notebook sections. Some integrations depend on third-party services, Windows applications, installed software, and provider availability.
