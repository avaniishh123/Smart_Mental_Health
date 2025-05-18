# **AI-Powered Mood Detection & Recommendation System**

## **Project Description**
This system detects the user's mood from their speech and provides personalized recommendations to improve their mood. It utilizes speech-to-text conversion, sentiment analysis, and voice tone analysis to identify moods and suggest relevant activities.

## **Features**
- **Speech-to-Text Conversion**: Converts speech to text using the Whisper ASR model.
- **Sentiment Analysis**: Analyzes the text to detect mood using a BERT-based NLP model.
- **Mood Recommendations**: Suggests activities based on detected mood (e.g., happy, sad, anxious, stressed).
- **Multi-Language Support**: Offers voice responses in different languages with Google Text-to-Speech (gTTS).
- **Voice Tone Analysis**: Analyzes pitch and tone of voice to enhance mood detection.

## **Installation**
To run the project locally, you need to install the dependencies. Run the following command to install the required libraries:

```bash
pip install -r requirements.txt
```

Or install manually using:

```bash
pip install openai-whisper transformers speechrecognition pydub torch pandas scikit-learn gtts deep-translator librosa nltk matplotlib
```

## **How to Use**

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/avaniishh123/mood-detection-system.git
   cd mood-detection-system
   ```

2. **Run the Code**: After installing the dependencies, run the Python script or Jupyter notebook to start using the system.
   
3. **Upload an Audio File**: The system will convert the speech in the audio file to text.

4. **Mood Detection**: It will analyze the sentiment of the text and detect the mood.

5. **Get Recommendations**: Based on the detected mood, the system will provide a list of mood-enhancing activities.

6. **Voice Response**: The system will use gTTS to speak the recommendations in your chosen language.

## **Example Workflow**

1. Record your voice and save it as an audio file (e.g., `mood_audio.wav`).
2. Run the system with the audio file as input.
3. The system detects whether you are feeling happy, sad, anxious, or stressed.
4. It recommends activities like "Music Therapy," "Yoga," or "Breathing Exercises" depending on the mood.
5. The system speaks back the recommendations in the selected language.

## **Code Walkthrough**
- **Speech-to-Text**: The `transcribe_audio()` function converts audio to text using Whisper ASR.
- **Sentiment Analysis**: The `analyze_sentiment()` function detects mood using a fine-tuned BERT model.
- **Recommendations**: The `recommend_activity()` function generates mood-specific activity suggestions.
- **Text-to-Speech**: The `speak()` function provides voice responses in multiple languages.

## **Dependencies**
- `openai-whisper`: For speech-to-text conversion.
- `transformers`: For sentiment analysis using BERT.
- `speechrecognition`: For basic audio processing.
- `gtts`: For text-to-speech functionality.
- `librosa`: For audio feature extraction and tone analysis.
- `deep-translator`: For multi-language translation.
- `nltk`: For natural language processing.
## **Demo Video**

Link:- https://drive.google.com/file/d/1y-IFiPYT51qRa3LPoEIvHgxyFLJ1l-LJ/view?usp=sharing

## **Contributing**
If you'd like to contribute to this project, feel free to fork the repository, make changes, and create a pull request. Please ensure that your code is well-tested and documented.

## **License**
This project is licensed under the MIT License.
