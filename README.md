# Speech-to-Text & Text-to-Speech Web Application

## Project Overview

A Flask-based web application that leverages Google Cloud Platform's AI services to provide speech-to-text and text-to-speech capabilities. The application allows users to record audio, get transcriptions, and generate synthetic speech from text input.

## Features

- **Speech-to-Text:**

  - Real-time audio recording through browser
  - Audio file upload support
  - Transcription using Google Cloud Speech-to-Text API
  - Sentiment analysis of transcribed text
  - Audio playback functionality

- **Text-to-Speech:**
  - Text input interface for speech synthesis
  - WaveNet algorithm for natural-sounding speech
  - Multiple voice options and languages
  - Download generated audio files
  - Audio file management system

## Tech Stack

- **Backend:**
  - Python 3.11.7
  - Flask Web Framework
  - Google Cloud Speech-to-Text API
  - Google Cloud Text-to-Speech API
- **Frontend:**
  - HTML5/CSS3
  - JavaScript (Browser Audio API)
  - Responsive Design
- **Cloud Infrastructure:**
  - Google Cloud Run
  - Google Cloud Storage

## Project Structure

```
cap5930_project1/
├── templates/
│   └── index.html          # Main web interface
├── app.py                  # Flask application
├── codes.ipynb            # Development notebook
├── STT.ipynb             # Speech-to-Text implementation
├── script.js             # Frontend functionality
├── requirements.txt      # Python dependencies
├── Dockerfile           # Container configuration
└── app.yaml            # Google Cloud deployment config
```

## Setup and Installation

1. Clone the repository

```bash
git clone [repository-url]
```

2. Install dependencies

```bash
pip install -r requirements.txt
```

3. Set up Google Cloud credentials

```bash
export GOOGLE_APPLICATION_CREDENTIALS="path/to/credentials.json"
```

4. Run the application

```bash
python app.py
```

## Usage

### Recording Audio

1. Click "Record an Audio" in the sidebar
2. Press the "Record" button
3. Speak into your microphone
4. Press "Stop" when finished
5. Wait for transcription and sentiment analysis

### Text to Speech

1. Click "Text to Audio" in the sidebar
2. Enter text in the textarea
3. Click "Generate Audio"
4. Play or download the generated audio file

## API References

- [Google Cloud Speech-to-Text API](https://cloud.google.com/speech-to-text)
- [Google Cloud Text-to-Speech API](https://cloud.google.com/text-to-speech)

## Deployment

The application is deployed on Google Cloud Run:

```
https://cap5930-project-1-image-servicename-286260167488.us-east4.run.app/
```

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a pull request

## License

[Specify License]

## Contact

[Your Contact Information]

## Acknowledgments

- Google Cloud Platform
- Flask Community
- Web Audio API Documentation
