# 788assignment5
# CRNN Text Recognition

This repository contains code for training and testing a CRNN (Convolutional Recurrent Neural Network) model for text recognition using PyTorch.

## Training

### Steps

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your_username/your_repository.git
   cd your_repository
mkdir data
# Download and extract the Num10k dataset into the data directory
pip install -r requirements.txt
python train.py --train_data data/train --valid_data data/val --output_dir saved_models --num_epochs 10 --lr 1.0 --batch_size 32 --imgH 32 --imgW 100
python test.py --saved_model path/to/saved_model.pth --valid_data data/val --batch_size 32 --imgH 32 --imgW 100
