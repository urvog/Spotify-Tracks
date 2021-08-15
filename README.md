# Analyzing Spotify Data Tracks - What makes a song a hit and popular?

Data Science Project - Analysis from Udacity Nano Degree Project I

## Motivation

In this project we are going to carry out an analysis of the attributes of a Spotify dataset in order to know what makes a song become a hit.

## Process

For the development of this project we will be using the CRISP-DM methodology, which include the following stages.
Business Understanding
Data Understanding
Prepare Data
Data Modeling
Evaluate the Results
Deploy

## Business Understanding

1. What features are necessary for a song to become a hit?
2. Is a song that sounds sadder or angry can be a hit??
3. What features are necessary for a song to be danceable.
4. Why Pink Floyd songs are not popular than the rest of the songs that are in the top?

The 6 phases aren't necessary for all the projects; a lot of questions can be answered without building models. In this post, I will apply CRISP-DM steps 1,2,3,5, and 6 to the Data Set.

## Installation

Librariesrequired:
- Python 3
- Scikit-learn
- Seaborn

## Dataset

Index(['id', 'name', 'popularity', 'duration_ms', 'explicit', 'artists',
       'id_artists', 'release_date', 'danceability', 'energy', 'key',
       'loudness', 'mode', 'speechiness', 'acousticness', 'instrumentalness',
       'liveness', 'valence', 'tempo', 'time_signature'],
      dtype='object')
      

- id: The Spotify ID for the track.
- name: name of the song
- popularity: Popularity fo the song. The value will be between 0 and 100, with 100 being the most popular. 
- durantion_ms: The duration of the track in milliseconds.
- explicit: Whether or not the track has explicit lyrics ( true = yes it does; false = no it does not OR unknown).
- artists: artist's name
- id_artist: The spotify artist ID
- release_date: The date the track was first released. 
- danceability: Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.
- energy: Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. For example, death metal has high energy, while a Bach prelude scores low on the scale. Perceptual features contributing to this attribute include dynamic range, perceived loudness, timbre, onset rate, and general entropy.
- key: The key the track is in. Integers map to pitches using standard Pitch Class notation . E.g. 0 = C, 1 = C♯/D♭, 2 = D, and so on.
- loudness:The overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track and are useful for comparing relative loudness of tracks. Loudness is the quality of a sound that is the primary psychological correlate of physical strength (amplitude). Values typical range between -60 and 0 db.
- mode: Mode indicates the modality (major or minor) of a track, the type of scale from which its melodic content is derived. Major is represented by 1 and minor is 0.
- speechiness: Speechiness detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value. Values above 0.66 describe tracks that are probably made entirely of spoken words. Values between 0.33 and 0.66 describe tracks that may contain both music and speech, either in sections or layered, including such cases as rap music. Values below 0.33 most likely represent music and other non-speech-like tracks.
- acousticness: A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.
- instrumentalness: Predicts whether a track contains no vocals. “Ooh” and “aah” sounds are treated as instrumental in this context. Rap or spoken word tracks are clearly “vocal”. The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content. Values above 0.5 are intended to represent instrumental tracks, but confidence is higher as the value approaches 1.0.
- liveness: Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A value above 0.8 provides strong likelihood that the track is live.
- valence: A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry).
- tempo: The overall estimated tempo of a track in beats per minute (BPM). In musical terminology, tempo is the speed or pace of a given piece and derives directly from the average beat duration.
- time_signature: An estimated overall time signature of a track. The time signature (meter) is a notational convention to specify how many beats are in each bar (or measure).

## Licensing

This project is published in 2021 under [MIT] (https://es.wikipedia.org/wiki/Licencia_MIT) license.
