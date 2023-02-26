# Image Classifier

This repository contains a deep learning model for classifying images using MobileNetV2 and transfer learning for optimization. The model is implemented in Keras from TensorFlow and is designed to be trained on custom image datasets.

## Table of Contents

- [Requirements](#requirements)
- [Usage](#usage)
- [Training](#training)
- [Contributing](#contributing)
- [License](#license)

## Requirements

To use the image classifier, you will need to install the dependencies listed in the `requirements.txt` file. You can do this by running the following command in the repository directory:

pip install -r requirements.txt


## Usage

To use the image classifier, first clone the repository to your local machine. Then, navigate to the repository directory and run the following command:

python predict.py --image path/to/image.jpg --model path/to/model.h5 --labels path/to/labels.txt


This will load the model from the specified file, predict the class of the input image, and output the result to the console.

## Training

To train the image classifier on a custom dataset, you will need to prepare the data in the format expected by Keras. This typically involves organizing the images into subdirectories based on their class, as described in the Keras documentation.

Once the data is prepared, you can train the model using the `train.py` script. This script provides several command-line options for configuring the training process, such as the number of epochs, the learning rate, and the batch size.

For example, to train the model on a dataset stored in the `data` directory for 10 epochs with a batch size of 32, you can run the following command:
python train.py --data_dir data --epochs 10 --batch_size 32


## Contributing

We welcome contributions to this repository, including improvements to the existing model and new features. To contribute, please fork the repository and submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
