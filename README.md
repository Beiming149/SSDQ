# SSDQ
SSDQ: Target Speech Extraction via Semantic and Spatial Dual Querying

This repository contains the official implementation of SSDQ, a framework for target speech extraction that leverages semantic and spatial dual querying strategies.


Start from building the environment

    pip install -r requirement.txt

## 🚀 Getting Started

### 1. Clone the Repository

    git clone https://github.com/Beiming149/SSDQ.git

    cd SSDQ

### 2. Install Dependencies

Make sure you are using Python 3.8+ and run:

    pip install -r requirements.txt

### 3.Datasets

We use SS-Libri as the main benchmark dataset for speech extraction tasks. Download directly from Hugging Face:

👉 SS-Libri Dataset:

Pending update...

After downloading, set the dataset root directory in config.yaml or pass it as an argument:

dataset_root: /data

### 4.Train

To train the SSDQ model from scratch:

    bash run.sh 

You can also resume training:

change run.sh  e.g.

    #!/bin/bash
    ...
    python train.py \
      --config config/train.yaml \
      --checkpoint_dir checkpoints/your_path \
      --train_from_last_checkpoint 1
  
###  Acknowledgements

This repo is built with reference to ClearerVoice. Thanks to the contributors of open source speech separation frameworks.
