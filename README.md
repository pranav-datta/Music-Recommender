Large music streaming services such as Spotify face challenges in effectively recommending songs to users. Currently, these platforms rely on creating listening profiles of their users and recommending songs based on the listening histories of similar users, without leveraging the intrinsic characteristics of the music itself for determining song similarity. To offer a different method for song recommendation systems, we conducted a comparative study of seven different deep learning models tasked with predicting a song’s genre based on raw audio.

For training, we used the popular GTZAN dataset which consists of 1,000 audio clips categorized by genre. To increase the size of the dataset, each clip was split into three separate audio files. Each file was then converted into a Mel-spectrogram, a graphical display of a song’s frequency and loudness with respect to time. The models featured in the comparative study are the following: LSTM, Trans- former encoder, 1D CNN, 2D CNN, 2D convolutional encoder, 1D convolutional encoder, and ResNet.

We tested each model with the Mel-spectrograms as the input and the target value being the respective song’s genre. Our results found that the LSTM and 1D convolutional encoder models exhibited the highest accuracy at approximately 70%. Considering its high accuracy in combination with low training times and robustness against hyperparameter values, we recommend the adoption of the 1D convolutional encoder architecture for music recommenda- tion systems.
