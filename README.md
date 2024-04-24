# Text-Summarization
This project implements a text summarization model using deep learning (LSTM) with an attention mechanism.

# Overview
Text summarization is the task of condensing a piece of text to its key points or main ideas. In this project, we use a sequence-to-sequence model with attention to perform abstractive text summarization.
The model consists of an encoder-decoder architecture with LSTM (Long Short-Term Memory) layers. The encoder processes the input text and generates context vectors, which are then used by the decoder to generate the summary.


# Model Architecture
Encoder:
Embedding Layer: Converts input text sequences into dense vectors.
LSTM Layers: Captures the sequential information of the input text.
Attention Layer:
Implements Bahdanau attention mechanism to focus on relevant parts of the input sequence.
Decoder:
Embedding Layer: Converts target summary sequences into dense vectors.
LSTM Layer: Generates the summary based on the encoder output and attention.
Training:
RMSprop optimizer is used with sparse categorical cross-entropy loss.
Early stopping is applied to prevent overfitting.
