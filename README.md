# Voice Virtual Assistant with NLP

This project was developed as a bootcamp challenge solution, implementing a hybrid virtual assistant in Python with:

- Speech-to-Text (voice to text)
- Text-to-Speech (text to voice)
- Intent classification using TF-IDF + cosine similarity
- Voice-triggered command execution through plugins (YouTube and Wikipedia)

Bootcamp reference: [Coding The Future BairesDev - Machine Learning Practitioner bootcamp](https://www.dio.me/bootcamp/coding-the-future-baires-dev-machine-learning-practitioner).

## Technologies and libraries

- Python 3.x
- `speechrecognition`
- `pyttsx3`
- `wikipedia`
- `scikit-learn`
- `nltk`
- `pyaudio`
- `IPython.display` (for the visual indicator in the notebook)

## Project structure

- `virtual-assistant.ipynb`: main notebook containing the full implementation.

## Implemented features

- Speech recognition module (`SpeechToText`)
- Speech synthesis module (`TextToSpeech`)
- Animated visual indicator for assistant states (listening, processing, speaking)
- Plugin system (`PluginLoader`)
- NLP intent engine (`IntentEngine`) using TF-IDF
- YouTube search plugin
- Wikipedia search/summary plugin

## How to run

1. Open the `virtual-assistant.ipynb` notebook in a Jupyter environment.
2. Install dependencies by running the installation cell:

```python
%pip install speechrecognition pyttsx3==2.71 wikipedia scikit-learn nltk pyaudio
```

3. Run the cells in order.
4. Start the main execution cell for the voice loop.
5. Speak commands such as:
   - "open youtube"
   - "search for a video on youtube about neural networks"
   - "search wikipedia for natural language processing"
6. To stop, say: `sair`.

## Notes

- The notebook is intended for local execution with an active microphone.
- On Windows, voice output may depend on the SAPI5 driver and installed system voices.
- Command accuracy depends on speech recognition quality and intent similarity.

## Challenge statement

### Challenge description

Creating a virtual assistant system from scratch.
In this project, a virtual assistant system must be developed using NLP (Natural Language Processing), based on the libraries presented during the course. The system must meet the following requirements:

- A module to transform text into audio (text to speech);
- A module to transform speech (human natural language) into text (speech to text);
- Module 2 must trigger, through voice commands, some automated functions, such as: opening a Wikipedia search, opening YouTube, and showing the location of the nearest pharmacy.

To complete this project, all libraries presented in the course may be used, especially the SpeechRecognition library in Python.

To help with the project, two examples are available, one for text to speech and one for speech to text. Both can be found on GitHub through the links below:

- Text to speech: https://github.com/diegobrunoDIO/Text-to-Speech-DIO
- Speech to text: https://github.com/diegobrunoDIO/Speech-to-text-ML-DIO

## References

- [Aula 8.py about nltk + TfidfVectorizer + cosine_similarity](https://github.com/FaculdadeDescomplica/Faculdade-Descomplica-Intelligent-Communication)
- [Processamento de Linguagem Natural - Silvio do Lago Pereira](https://www.ime.usp.br/~slago/IA-pln.pdf)