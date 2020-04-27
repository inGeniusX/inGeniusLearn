# inGeniusLearn
inGeniusLearn by inGenius X: 
A deep learning powered application that hyperpersonalizes educational experience by analyzing your facial stress indicators and providing topic advice during a short, non-invasive diagnostic.

# Usage
1. Select a video lecture that you want to learn from.
2. The moment you click on play button, emotion detection model kicks in and continuously monitors your behavior.
3. When the model detects that the user is stressed/confused for few continuous frames it pauses the video, analyse the transcripts of the video upto the exact time when the user seemed confused.
4. The model looks few moments into the future and past and recommend topics that might have confuseed the user. The text analays model does this by learning distributed representations form the wikipedia text of the topic and comparing the similarity of the words in the transcripts.
5. These topics are then presented to the user with a brief description abut each of them, giving user time to understand them before they jump to other advanced concepts deep into the video.

# Models and Functions
1. CNN model: Convolution Neural Net for non-invasive stress detection through facial analysis trained on [FER-2013 dataset](https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data). Certain classes were merged to create new expressions so that there are 4 classes HAPPY, NEUTRAL, CONFUSED, STRESSED.[Trained model](https://drive.google.com/open?id=1MNhezLab0lH2n4GLV4wb8icycJKZpggR)
2. Text analysis: Provides personal topics depending upon the factors of stress detection during the diagnostic.

# libs and languages
1. Tensorflow-gpu(1.7): for creating and training CNN.
2. Flask: For deplopyment.
3. OpenCV: face-detection.
4. YouTube transcript API: To get transcripts for a given video.
5. Python, Javascript and HTML.
