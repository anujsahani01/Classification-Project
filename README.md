# Intent and Entity Extraction and Classification from audio files

![image](https://github.com/anujsahani01/Classification-Project/assets/83875986/bcac58b0-ca64-4ef8-aa85-6a237d69b513)


## Description: 

The objective of this project is to develop a system that performs intent and entity extraction from audio files. The system involves converting speech to text while incorporating speaker recognition, and utilizes pretrained models from the 🤗 (Hugging Face) library for entity and intent classification. The end result is a JSON file containing the audio data, along with accurately identified intents and classified entities.


## Project Overview:

* **Speaker Recognition:** In this stage, the pyannote/voice-activity-detection model is employed. This model follows a two-stage process. First, it extracts relevant features from the audio signals. Second, a classification algorithm is applied to these extracted features, resulting in the identification of the speaker.
  
* **Speech to Text conversion:** The jonatasgrosman/wav2vec2-large-xlsr-53-english model is used for converting speech to text. This model is based on Facebook's wav2vec2 model and has been fine-tuned for speech-to-text conversion. It comprises a speech-to-text processor that combines a feature extractor and a tokenizer. The audio is tokenized into numpy arrays or tensors, producing a textual representation of the speech.
  
* **Intents Recognition:** Intent recognition is accomplished using the qanastek/XLMRoberta-Alexa-Intents-Classification model. This model is trained on a large dataset of text data that is labeled with specific intents. It is capable of classifying the extracted text into predefined intent categories, providing insight into the purpose or goal behind the spoken words.
  
* **Entity Recognition and Classification:** The huggingface-course/bert-finetuned-ner model is employed for entity recognition and classification. This model is trained on extensive text data where entities are labeled. It is able to identify and classify various entities present in the extracted text, such as names, dates, locations, and more. By utilizing this model, the system accurately recognizes and categorizes entities within the spoken text.

## Used following 🤗models for performing tasks:

* **pyannote/voice-activity-detection:** This model performs speaker recognition by extracting useful features from audio signals and applying a classification algorithm to determine the speaker's identity.

* **jonatasgrosman/wav2vec2-large-xlsr-53-english:** This model is specifically designed for speech-to-text conversion. It is based on Facebook's wav2vec2 model and includes a speech-to-text processor that combines feature extraction and tokenization to convert audio into numpy arrays or tensors.

* **qanastek/XLMRoberta-Alexa-Intents-Classification:** This model is trained on a large corpus of text data with labeled intents. It can classify the extracted text into different intent categories, providing insight into the purpose behind the spoken words.

By utilizing these pretrained models and combining the different stages, the system can accurately extract intents and entities from audio files. The resulting JSON file provides a structured representation of the audio data, along with the associated intents and entities. This enables further analysis and processing of the audio content in various domains, such as voice assistants, call center analytics, and automated transcription services.


## Feedback

If you have any feedback, please reach out to me at: [![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/anuj-sahani-34363725b) 

Author: [@anujsahani01](https://github.com/anujsahani01)

