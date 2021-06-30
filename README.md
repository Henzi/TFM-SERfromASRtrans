# TFM-SERfromASRtrans
EMOTION RECOGNITION FROM SPEECH TRANSCRIPTIONS
Many techniques and systems exist to try recognizing emotion in speech. 
However, most of them are only used to detect emotion from english speech.
Very few developed research on speech emotion recognition are actually trained using Spanish datasets.
Our implemented system recognizes emotions from the transcriptions predicted by a spanish automatic speech recognition model. 
The triphone GMM-HMM is used as the ASR model. 
It is implemented and trained from scratch with the help of a new wrapper, ExKaldi, 
which allows using Kaldi open-software with only python as a programming language, thus avoiding learning Kaldi command format.
The SER model extracts linguistic features through pre-trained word2vec and performs the classification with a decision tree algorithm.
Our experiments show that spanish speech emotion recognition through automatic speech transcription is not accurate if the dataset used 
to classify the SER model is small (less than 400 audio samples) with short-length audio samples (around 3.5 seconds).
Results also show that the ASR model reaches more accurate transcription predictions when  speaker adaptive training is added.

In order to be able to run the code all the paths must be changed. The Kaldi, ExKaldi and all required libraries must be installed preferently in a virtual environment.
The datasets used are not published in here. 
