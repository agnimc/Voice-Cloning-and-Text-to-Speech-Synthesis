# Voice-Cloning-and-Text-to-Speech-Synthesis
We implement a neural-network based system to perform Voice Cloning and Text-to-Speech
(TTS) synthesis that is able to clone voice of different speakers, including both trained and
untrained voice samples. Our system consists of three modules, each been trained
independently: (1) a Speaker Encoder network, which is trained on a speaker verification task
using an autonomous dataset of speech samples without transcripts from different speakers, to
generate a fixed-dimensional embedding vector from only few seconds of reference speech
from a chosen speaker; (2) a Synthesizer sequence-to-sequence network inspired from
Tacotron 2 which generates a mel-spectrogram from text of our choice based on the speaker;
(3) A Vocoder network based on an auto-regressive WaveNet that converts the melspectrogram
into audio waveform samples from text provided by the user, thus performing
TTS. Through this, we are able to demonstrate that our proposed model is able to transfer its
knowledge of speaker variability, which it learns from the speaker encoder trained
discriminately, to the multispeaker Text-to-Speech task. After that, it is able to synthesize the
natural speech of the selected speaker and other speakers that are not trained in the network.
We enumerate the importance of training the speaker encoder on a large and assorted speaker
dataset in order to obtain the best generalization performance. Finally, we show that randomly
sampled speaker embeddings, either recorded or imported, can be used to synthesize speech in
the voice of new speakers different from those used in training, indicating that the model has
learned a high quality speaker demonstration. Our work is done on a SV2TTS (Speaker
Verification to Text-to-Speech Synthesis) Toolbox written in Python which is able to combine
the three independent models into one single model in order to provide the best performance
on the embedded dataset selected by the user. We make use of both CPU and GPU support to
facilitate the different operations of our model and smoothen the process for the user. The
toolbox also generates plots of the synthesized voices that can be used to differentiate between
two voice samples, or between two utterances of the same speaker, which can be both novel
and synthesized. All the work is done in Real-Time for the ease of the user. In this report, we
talk about the implementation of our model, and how its methodology and design vary from
related works in this area and what the future holds for this technology.
