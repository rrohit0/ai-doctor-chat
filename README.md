# AI Doctor Chatbot

The AI Doctor Chatbot is an advanced system designed to assist users with medical inquiries by mimicking a doctor's interaction through AI-driven speech and text processing. It can evaluate patient symptoms, offer preliminary medical guidance, and support virtual healthcare consultations.

## Technologies Used

- **Eleven Turbo v2** for high-quality speech synthesis and interactive voice communication.
- **Llama-3.2-90B-Vision-Preview** for sophisticated natural language comprehension and visual data analysis.

# Project Setup Instructions

This guide outlines the necessary steps to configure the AI Doctor Chatbot environment, including installing required dependencies and launching the application.

## Installing FFmpeg and PortAudio

### Windows

#### Setting Up FFmpeg

1. Download FFmpeg:
   - Visit the [FFmpeg Downloads](https://ffmpeg.org/download.html) page.
   - Go to the Windows builds section and get the latest static version.

2. Extract and Configure FFmpeg:
   - Unzip the downloaded file into a directory, such as `C:\ffmpeg`.
   - To update your system's PATH:
     - Search for "Environment Variables" in the Start menu.
     - Click "Edit the system environment variables."
     - Under "System Properties," select "Environment Variables."
     - Locate the "Path" variable under "System variables" and click "Edit."
     - Click "New" and enter the path to the `bin` folder (e.g., `C:\ffmpeg\bin`).
     - Click "OK" to save the changes.

#### Installing PortAudio

1. Download the PortAudio binaries from the [official website](http://www.portaudio.com/download.html).
2. Follow the provided installation guide to complete the setup.

## Setting Up API Keys

1. Create a `.env` file in the root directory of your project.
2. Open the `.env` file and paste your API keys in the following format: 
3. Save the file and ensure it is loaded correctly in your application.


## Configuring a Python Virtual Environment

### Using Pipenv

#### Install Pipenv (if not already installed):
```sh
pip install pipenv
```

#### Install Dependencies with Pipenv:
```sh
pipenv install
```

#### Activate the Virtual Environment:
```sh
pipenv shell
```

### Using pip and venv

#### Create a Virtual Environment:
```sh
python -m venv venv
```

#### Activate the Virtual Environment:
```sh
venv\Scripts\activate
```

#### Install Required Packages:
```sh
pip install -r requirements.txt
```

## Running the Chatbot

### Phase 1: Core AI Processing (Doctor's Brain)
```sh
python brain_of_the_doctor.py
```

### Phase 2: Patient's Speech Input
```sh
python voice_of_the_patient.py
```

### Phase 3: Doctor's Speech Output
```sh
python voice_of_the_doctor.py
```

### Phase 4: Deploying the Gradio Interface
```sh
python gradio_app.py
```

