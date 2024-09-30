## Variational Autoencoder (VAE) Implementation using PyTorch Lightning

### Overview
This repository contains a PyTorch Lightning implementation of a Variational Autoencoder (VAE), designed for generating new data that mimics the input data distribution. The VAE can be trained on various datasets and is capable of learning latent representations of the input data.

### Installation
To run this project, you need Python 3.x and PyTorch along with PyTorch Lightning. You can install the dependencies via pip:
```python
pip install pytorch-lightning
pip install torch
pip install torchvision
pip install matplotlib
pip install pandas
pip install numpy
```

### Code Structure
1. **Environment Setup**: Initial setup for installing necessary libraries and dependencies.
2. **Data Loading**: Code to load and preprocess data using PyTorch's DataLoader and torchvision transforms.
3. **Model Definition (PyTorch Lightning)**:
   - **LightningModule**: Defines the VAE model, including methods for the forward pass, loss computation, and the training/validation steps. Utilizes PyTorch Lightning's module structure to encapsulate all model-related logic, making it modular and easy to maintain.
   - **Trainer**: Manages the training process, leveraging PyTorch Lightning's Trainer class for handling device placement, logging, and validation/testing loops, simplifying the training code and enhancing reproducibility.
4. **Training**: Setup for training the model, including optimizer configuration and training loops, all managed by the PyTorch Lightning Trainer which abstracts the complexity of manually handling these elements.
5. **Visualization**: Utilities to visualize the results of the VAE, including functions to display original and reconstructed images.

### Usage
To train the VAE model, simply run the notebook cells sequentially. Ensure that the dataset paths and other configuration settings are adjusted according to your environment.

Some functions have their detailed mathematical explanation commented above/below them

If you run the files locally your output and the loss gets saved automatically locally. But I also added a print statement for logger for each iteration of the for loop in the `training_step` function so that the output can be displayed in the jupyter output logs.


### Contributing
Contributions to this project are welcome. Please fork the repository and submit a pull request with your suggested changes.


Feel free to ask me anything on [twitter](https://x.com/parthshr370) or [LinkedIn](https://www.linkedin.com/in/parthshr370/)
