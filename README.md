# EmotionDetectionAudio
Emotion Detection using Audio files

Steps to run the project
1) Extract the code.zip file to retrieve the dataset related to the project
2) Upload all the files into google colab including code folder
3) mount the google drive folder in the colab and copy the path of the code folder which you uploaded into the google drive
4) now adjust the code folder path in both the ipynb files.
5) Now Run the code in the google colab.
6) Added the code documentation as well for detailed walkthrough of code and running the project



Code Documentation:

Platform: Google Colab 
Programming Language: Python
Data Set: Kaggle (RAVDESS) dataset with 1440 files.
Model: CNN model.
Emotion Detection using Audio files
Steps to run the project

1)  Extract the code.zip file to retrieve the dataset related to the project

2) Upload all the files into google colab including code folder
mount the google drive folder in the colab and copy the path of the code folder which you uploaded into the google drive

Note: Make sure the paths in the reading directory and create dataframe are as per your google drive link
Example of my link: os.listdir('/content/drive/MyDrive/EmotionDetectionAudio-main/EmotionDetectionAudio-main/code/code')

3) Now adjust the code folder path in both the ipynb files.

4) Now Run the code in the google colab.

We have kept all the required audio file in the google drive and mounted the drive for data extraction and access to the data.
Make sure to install the required packages numpy, matplotlib, pandas, librosa, resampy, seaborn, scipy, tensorflow, keras using the pip install.  This we have taken care by adding the initial cell. This is followed by importing the required libraries/ packages from  keras, sklearn, scipy etc. Also import the packages required for data visualization like matplotlib, seaborn etc. We have imported librosa for cleaning the data and o concentrate on the front end pitch.

Once completing the installing and importing the required libraries, read the dataset (Audio files from different actors) by creating the data frame. This if followed by defining the features of the dataset including gender, intensity, statement, repeat, emotion etc.

We have printed the dataset using .head().

Next for data exploration we have plotted the audio file’s waveform ad spectrogram using librosa and matplotlib.

We have also plotted the Mel Power Spectrogram using librosa and matplotlib.

We used MFCC to extract the features from the audio files. The MFCC plot was created using librosa and matplotlib.

Next we have defined the truth labels for the dataset and displayed it using .head().

Next we have plotted the Emotion Distribution Histogram for the dataset using seaborn. This was followed by data splitting for male and female actors.

After this we have extracted the features from the audio files using librosa with MFCC. We used data augmentation to enhance the dataset since the number of audio files were not sufficient for training the model. We have stretched the files, added noise, altered pitch etc. for this. The raw waves for these files were plotted using IPython.display.
This augmented data was then combined with the original data.

The next step included changing the dimension for the CNN model using Numpy and Keras. The evaluation metrics were defined using Keras. We have used precision, recall and F1 score here. We have printed the model summary next.

After this we have removed the training part to avoid unnecessary long epoch lists. We then saved the model and predicted the emotions on test data.

We have used a random baseline model to compare the performance of our model. We have printed the confusion matrix and evaluation metrics. The final accuracy comes to 86% and the baseline accuracy comes to 18%.

Emotion Detection using Audio files
Steps to run the project

1)  Extract the code.zip file to retrieve the dataset related to the project

2) Upload all the files into google colab including code folder
mount the google drive folder in the colab and copy the path of the code folder which you uploaded into the google drive

Note: Make sure the paths in the reading directory and create dataframe are as per your google drive link
Example of my link: os.listdir('/content/drive/MyDrive/Deep Learning/Emotion Detection using Audio/code')

3) Now adjust the code folder path in both the ipynb files.

4) Now Run the code in the google colab.






