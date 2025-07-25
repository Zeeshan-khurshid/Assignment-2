# Assignment-2
Encoder-Decoder Models using RNN and LSTM
<h1>Model structure </h1>
<p>
The proposed model for English-to-French translation is based on a Sequence-to-Sequence (Seq2Seq) architecture implemented using Recurrent Neural Networks (RNNs), specifically Long Short-Term Memory (LSTM) units.

The architecture comprises two primary components:

Encoder:
The encoder processes the input English sentence. It includes an Embedding layer that converts input tokens into dense vector representations, followed by an LSTM layer that captures the temporal dependencies within the input sequence. The encoder outputs its internal states—hidden and cell states—which are used to initialize the decoder.

Decoder:
The decoder generates the translated French sentence. It also begins with an Embedding layer, followed by an LSTM layer that takes the encoder’s final states as its initial states. The decoder predicts each word step-by-step, and a Dense layer with softmax activation is used to produce a probability distribution over the target vocabulary at each time step.

The model is trained using the categorical cross-entropy loss function and optimized with an appropriate optimizer such as Adam. The training process monitors accuracy as the key performance metric.

This architecture enables the model to learn meaningful alignments between input and output sequences without the use of explicit attention mechanisms.
</p>
