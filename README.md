# ASR - PyTCI
<hline>

## Introduction
<hline>

> Paper implemented: Understanding Adaptive, Multiscale Temporal Integration In Deep Speech Recognition Systems [https://openreview.net/pdf?id=h4es0CIohF](url)

Understanding how deep neural networks (DNNs) integrate information across different timescales is crucial for tasks like speech recognition. Temporal Context Invariance (TCI) paradigm is introduced to investigate this integration in DNNs.

### Key Findings:

* DNNs exhibit a hierarchical integration of information across time.
* We find that most model units, including those in recurrent layers, have distinct integration windows.
* Training causes these integration windows to evolve: shrinking at early layers and expanding at higher layers.
* There's a transition point where integration windows align with the duration of speech structures (e.g., phonemes or words).
* Both recurrent and convolutional networks show similar integration patterns, with recurrent networks emphasizing structure-yoked integration.

These findings shed light on how DNNs encode the hierarchical structure of speech, aiding in the development of more effective speech recognition systems.

## Installation
<hline>
Create a virtual environment and install the necessary libraries.
  
```
conda create -n PyTCI python=3.10.12
conda activate PyTCI
conda install pytorch==2.2.1 torchvision==0.17.1 torchaudio==2.2.1 pytorch-cuda=12.1 -c pytorch -c nvidia
pip install matplotlib
pip install omegaconf
pip install git+https://github.com/SeanNaren/deepspeech.pytorch.git
pip install hydra-core
pip install lightning
pip install python-Levenshtein
pip install git+https://github.com/naplab/PyTCI.git
sudo apt-get install -y libsox-dev
```

Download the speech audio clips from [https://github.com/naplab/PyTCI/blob/main/Examples/resources.tar
](url) and extract them





## Implementation
<hline>


