# Task-Aware Graph Convolutional Network for Active Learning (TA-GCNAL)
PyTorch implementation of TA-GCNAL. For details, read the paper.

## Setup
The dependencies are in [`requirements.txt`](requirements.txt). Python=3.8.3 is recommended for the installation of the environment.


## Datasets
The code supports torchvision built-in implementations of MNIST, EMNIST and openml datasets.

## Training
For running an AL strategy in a single setting, use the following script that by default uses 5 different initial random seeds for the specified setting. 
```python
python main.py --data_name MNIST --data_dir your_data_directory --n_init_lb 100 --n_query 100 --n_round 15 --learning_rate 0.001 --n_epoch 1000 --model mlp --strategy CDALSampling
```

