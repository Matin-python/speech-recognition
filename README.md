# 🎙️ Speech Recognition using Python

A Python speech recognition project that converts spoken Persian language from an audio file into text using the SpeechRecognition library and Google's Speech Recognition service.

## Overview

This project demonstrates how to process an audio file and convert speech into written text.

The program loads a `.wav` audio file, records the audio data using the `SpeechRecognition` library, and sends the audio to Google's Speech Recognition service for transcription.

The project is currently configured to recognize **Persian (Iranian)** speech using the `fa-IR` language setting.

## Features

* 🎙️ Speech recognition
* 🔊 Audio file processing
* 📝 Speech-to-text conversion
* 🇮🇷 Persian language recognition
* 🎧 WAV audio file support
* ☁️ Google Speech Recognition service
* 🐍 Simple Python implementation

## Technologies Used

* Python
* SpeechRecognition
* Google Speech Recognition API

## Input

The program uses a WAV audio file as its input:

```text
tf.wav
```

The audio file contains the speech that will be converted into text.

The current project is configured for Persian speech recognition:

```python
text = r.recognize_google(audio, language='fa-IR')
```

The `fa-IR` language code specifies Persian as the recognition language.


## How It Works

The project follows these main steps:

```text
Load WAV Audio File
        ↓
Create Recognizer
        ↓
Read Audio Data
        ↓
Send Audio to Google
        ↓
Recognize Persian Speech
        ↓
Convert Speech to Text
        ↓
Print Result
```

## Speech Recognition

The `SpeechRecognition` library is used to process the audio.

First, a recognizer object is created:

```python
import speech_recognition as sr

r = sr.Recognizer()
```

The WAV file is then loaded:

```python
voice = sr.AudioFile("tf.wav")
```

The audio data is recorded from the file:

```python
with voice as source:
    audio = r.record(source)
```

The resulting audio object can then be sent to the speech recognition service.


## Contributing

Contributions, suggestions, and bug reports are welcome.

Feel free to fork this repository and submit a pull request.

## License

This project is licensed under the MIT License.

## Author

Mohammad Reza Bakhshandeh

Interested in Python, Machine Learning, Deep Learning, Computer Vision, Artificial Intelligence, and Game Development.
