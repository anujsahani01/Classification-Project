# Intent and Entity Extraction and Classification from audio files

## Convert speech to text along with speaker recognition then uses 🤗 pretrained models for Entity and Indent Classification in the extracted text, finally creating a json file of whole audio along with proper intents and entity.

This project is divided in 4 major parts
* Speaker Recognition
* Speech to Text conversion
* Intents Recognition
* Entity Recognition and Classification

## Used following 🤗models for performing tasks

1) pyannote/voice-activity-detection: Such models/algorithms are divided into two stages, in first step useful features are extracted from audio signals and in second step a classification algorithm is applied on the extracted features which results in final decision or classification of speaker.


2) jonatasgrosman/wav2vec2-large-xlsr-53-english: This is a speech to text converting model and is finetuned on facebook's wav2vec2 model. These models have a speech to text processor which is a combination of speech to text feature extractor and a tokenizer, which tokenize the audio in a numpy array or tensors.


3) qanastek/XLMRoberta-Alexa-Intents-Classification and huggingface-course/bert-finetuned-ner: These models were used for intent and entity recognization and classification. These models are trained on large text data having intent and entity classified.


