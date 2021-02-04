# Voice-Cloning-and-Text-to-Speech-Synthesis
What is needed?
Hardware:
 An NVIDIA graphics card which supports CUDA v10.0
Supported list of graphic cards
AMD graphic cards are not supported

Software:
Following software is needed along with their respective versions.
 pip
 Python 3.7
 PyTorch for CUDA 10.0
 NVIDIA CUDA 10.0
This particular version is needed since TensorFlow >=1.10.0, <=1.15 is required.


 NVIDIA cuDNN for CUDA v10.0
An NVIDIA developer account is needed to download this from the official website.
However, the software packages are also available as open source on the web.
 FFmpeg

PyTorch, CUDA and cuDNN are required to enable GPU support for the Synthesizer. GPU
drivers need to be properly installed and you have to make sure that your CUDA version
matches your PyTorch and Tensorflow installations. Enabling GPU support is a lot of work
and therefore optional.
After these have been installed, the following dependencies are required to run the toolbox:
 tensorflow==1.15
 umap-learn
 visdom
 librosa>=0.5.1
 matplotlib>=2.0.2
 numpy>=1.14.0
 scipy>=1.0.0
 tqdm
 sounddevice
 SoundFile
 Unidecode
 inflect
 PyQt5
 multiprocess
 numba==0.48

We will add the names of these dependencies in a .txt file along with the versions (wherever
needed) and name it dependencies.txt.
