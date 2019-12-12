# MusicRecmSystem
Music Recommendation using Machine Learning
The “Music Recommendation System” is meant to work as a music player which is capable of adding similar songs to the playlist based on the genre of the initial song played by the user. This feature is helpful in recommending the user some new songs which he might like as they are similar to the song played by him.
ML-based classification algorithms are used for predicting the genre of the song chosen and then this genre is used to search for similar songs from a collection (whose genre is already known). The names of this collection of songs contain the genre itself as part of the name, this fact is helpful for validation as we can check whether the genre of all the songs added to the playlist is same and is similar to the genre obtained by applying our classification model upon the song initially played
# Choice of Dataset
Our project focuses on getting data from the audio dataset for implementing Content based Filtering. In this project, our choice of Dataset is GTZAN Dataset. GTZAN Dataset contains 1000 songs of 30 seconds which is equally divided in to 10 genres. Other Datasets that could have been used is Million Songs Dataset (MSD) and Free Music Archive (FMA). We continued with GTZAN Dataset for our convenience since it had 10 different genres to deal with.

# Feature Generation
Each one of audio files from the dataset was taken and converted into equivalent spectograms. Spectogram can be defined as a visual representation of the complete spectrum of all the frequencies with respect to time. It can be seen as squared magnitude of short-term Fourier Transform (STFT) of the input audio signal. A Fourier transform is basically a representation that inputs a signal in time domain and outputs in frequencies. Mel Scale Spectogram uses Mel Scale in the y-axis to get Frequencies in different bins. This Mel scale Spectogram generation requires librosa built in library which directly converts an audio input into this. The function takes some parameters like – window length (window of time to perform transform) and hop length (number of samples between successive frames). We have used a window length of 2048 (appx 10ms). Hop length was taken as 512. Using Mel scale, we can distinguish between audio better as it scales the Hz scale using log function into dB (Decibels) and squashes the difference to relate more to human perceived pitch.


Refer to the Project Report Doc for more info.









