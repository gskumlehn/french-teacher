    # Wikipedia Search Audio (French Teacher)

This project allows you to perform Wikipedia searches in English using voice commands, automatically translate the results into French, and listen to the translated text as audio.
It is designed to help learners of French practice comprehension by hearing short summaries on various topics.

## Features

* **Voice Input (English)** – Speak into your microphone to define the search term.
* **Wikipedia Search (EN)** – Retrieves a short summary in English from Wikipedia.
* **Automatic Translation (EN → FR)** – Translates the summary into French.
* **Text-to-Speech in French** – Generates audio output of the translated text using Google Text-to-Speech (gTTS).
* **Audio Playback** – Plays the French translation so you can listen and improve pronunciation and comprehension.

## How It Works

1. The program open voice recordings and uses **SpeechRecognition** with Google Speech API to transcribe it into English text.
2. It searches for the spoken term on **Wikipedia** (English version) and fetches a short summary.
3. The summary is translated into French using **googletrans**.
4. The translated text is converted into speech using **gTTS**.
5. The French audio is played back to the user.

## Requirements

This project is intended to run in **Google Colab**.
The following Python packages are required:

* `gTTS`
* `wikipedia`
* `googletrans==4.0.0-rc1`
* `SpeechRecognition`
* `pydub`
* `pyaudio`

## Usage

1. Run the notebook cells to install dependencies and load the functions.
2. Add voice recording in english.
3. Wait for the script to:

   * Recognize your voice
   * Search Wikipedia
   * Translate the result into French
   * Generate and play the French audio

Example flow:

```
🎤 Say: "Eiffel Tower"
📝 Wikipedia summary (EN) → translated to FR
🔊 Plays: "La tour Eiffel est un monument..."
```

## Purpose

The main goal is to provide an **interactive French learning tool** where learners can:

* Expand vocabulary
* Hear correct pronunciation
* Explore different topics through Wikipedia
