# Music_genre_classification_chatbot

### INTRODUCTION

A music genre is a conventional category that identifies some pieces of music as belonging to a shared tradition or set of conventions (rock, pop, metal, etc). It is to be distinguished from musical form and musical style. 

Music can be divided into different genres in many different ways. The artistic nature of music means that these classifications are often subjective and controversial, and some genres may overlap. [1]

### DATASETS
#### GTZAN GENRE COLLECTION
This dataset was used for the well-known paper in genre classification “Musical genre classification of audio signals” by G. Tzanetakis and P. Cook in IEEE Transactions on Audio and Speech Processing 2002. [2]
As it can be seen in the Table 1 drawn below the dataset consists of 1000 audio tracks each 30 seconds long. It contains 10 genres, each represented by 100 tracks. The tracks are all 22050Hz Mono 16-bit audio files in .wav format.

#### CHATBOT DATASET 
To train the model built for the chatbot, a custom dataset that comprised of a file with 6 primary tags (“greeting”, “goodbye”, “age”, “name”, “shop”, “hours”). For each tag, there were appropriate patterns and responses that define a conversation and a few possible questions and answers a conversation may have. 

### MODELS
#### 	Music Genre Classification Model
A classification model built using Convolutional Neural Networks [3] through the Keras [4] [5] library, was used to classify the audio files according to the 10 genres as per the GTZAN Dataset [2]. The model we created yielded a test accuracy of approximately 68%, which in comparison with the other models built for the same purpose, is quite efficient. 

#### ChatBot Model
The ChatBot being the parent framework for the project, is built using a Deep Neural Network [3] through the tensorflow and tflearn libraries. A custom dataset of .json format was used to train the model using Natural Language Tool Kit (NLTK). The chatbot simulates a conversation with the user and for a particular message, it runs and shows the results of the Music Genre Classifier.

#### References
[1]https://en.wikipedia.org/wiki/Music_genre

[2] George Tzanetakis and Perry Cook. 2002. Musical genre classification of audio signals. IEEE Transactions on speech and audio processing 10(5):293– 302.

[3] J. Salamon and J. P. Bello, "Deep Convolutional Neural Networks and Data Augmentation for Environmental Sound Classification," in IEEE Signal Processing Letters, vol. 24, no. 3, pp. 279-283, March 2017, doi: 10.1109/LSP.2017.2657381. 

[4] Vyas G., Dutta M. K., “Automatic Mood Detection of Indian Music Using MFCCs and K- means Algorithm”, Seventh International Conference on Contemporary Computing (IC3), 2014 IEEE.

[5] K. Choi, D. Joo, and J. Kim, “Kapre: On-GPU Audio Preprocessing Layers for a Quick Implementation of Deep Neural Network Models with Keras,” 2017, [Online]. Available: http://arxiv.org/abs/1706.05781.
