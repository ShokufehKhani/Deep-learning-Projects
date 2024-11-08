### **Music Generation using RNNs**
This project demonstrates how to generate musical notes using a Recurrent Neural Network (RNN). We train the model using the MAESTRO dataset, which contains a large collection of piano MIDI files, to predict the next note in a sequence. By calling the model iteratively, we can generate longer compositions of music.

**Project Overview**

**Goal**
To create a generative music model using RNNs that can output a sequence of musical notes longer than 3 seconds.

**Approach**
1. Data Preprocessing: Parse and process MIDI files from the MAESTRO dataset to prepare training sequences.
2. Model Architecture: Use a recurrent neural network (Simple RNN or LSTM) to predict subsequent notes in a musical sequence.
3. Generation: Once trained, generate music by feeding the model an initial sequence of notes and predicting the following notes iteratively.

**Dataset**
The project uses the MAESTRO dataset, a dataset of piano performances in MIDI format. Each MIDI file represents a sequence of musical notes and durations, ideal for training an RNN model to learn note sequences.

**Dataset Link**
The MAESTRO dataset can be downloaded from: MAESTRO Dataset

**Prerequisites**
Python 3.x
TensorFlow
music21 (for handling MIDI files)
Install the necessary packages with:

**Code Structure**
- Data Loading: Parse and preprocess MIDI files to extract sequences of notes.
- Model Training: Train an RNN (Simple RNN, LSTM) on the preprocessed data to learn the note sequences.
- Music Generation: Generate new music sequences using the trained model.

**Training**
1. Load and preprocess MIDI files from the MAESTRO dataset.
2. Build and compile the RNN model.
3. Train the model for multiple epochs (suggested: >10) until it learns the note sequences well.

**Generating Music**
After training, you can generate music by:

1. Providing an initial seed sequence.
2. Using the trained model to predict and extend the sequence.
3. Saving the generated sequence as a MIDI file.

**Evaluation**
Model performance can be evaluated with standard metrics like accuracy during training, and qualitative results can be assessed by listening to the generated MIDI output.

**Output**
Generated music sequences are saved as MIDI files. The output file will contain a unique sequence of notes learned by the model from the training data.
