# MusicGenreClassification

介紹：https://drive.google.com/file/d/1pfpDK3ToswrLq0RI65SopvH7DNHIN4cv/view?usp=sharing

## Introduction: <br />
This project focuses on classifying music genres using convolutional neural networks, specifically employing the ResNet50V2 architecture.

## Data Description: <br />
The dataset utilized in this project is sourced from GTZAN (https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification?select=Data), accessible here. We have narrowed our focus to five primary genres: Jazz, Rock, Hip Hop, Country, and Classical. Each genre consists of 100 audio samples. To construct our training and testing sets, we have allocated 85% of the data for training, resulting in 425 audio samples, and 15% for testing, resulting in 75 audio samples.

## Pipeline (Steps): <br /> 
Preprocessing:
1. Loading Audio Files: Utilize the librosa library to load audio files, considering only the first 25 seconds of each track.
2. Conversion to Mel Spectrogram: Convert the audio data into mel spectrograms, representing the frequency content of the audio signal over time.
3. Rescaling: Rescale the mel spectrograms to fit within the range of 0 to 255, ensuring compatibility with RGB representation.
4.Representation in RGB Format: Transform the mel spectrograms into RGB format for compatibility with convolutional neural networks.

Melspectrogram in RGB with different gerne:

## Training: <br />
1. Data Splitting: Split the preprocessed data into training and testing sets with a ratio of 85:15.
2. Model Selection: Employ ResNet50V2 architecture augmented with dense layers to construct the classification model.

## Result: <br />
The accuracy achieve 75% at the end.
