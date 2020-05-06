[![Travis](https://img.shields.io/badge/language-Python-red.svg)]()

# Arabic_MNIST_Character_Classification
## Objective
In the well studied MNIST dataset the challenge was to recognize handwritten characters. Due to the rapid progress in machine learning, it is now possible to solve this task with an accuracy of almost 100%. This has inspired a research team (see Acknowledgements) to tackle the recognition of Arabic letters. The Arabic alphabet has 28 characters. Depending on where the letter is in the word, the spelling changes. 
<br>
At the time the research results were published, the state-of-the-art accuracy was 94.1%.
Our goal is to surpass this result by using modern methods and, above all, as little effort as possible.
In this notebook, we describe the entire process from data preparation/preprocessing to training the network using transfer learning and fine-tuning. Finally we will analyze the classification performance and present the results. 

## Dataset
The Dataset contains 16800 images of handwritten characters from the Arabic alphabet. Each image has the size of 32x32 pixel. 
The training set (13440 images, 490 images per character) and the validation set (3360 images, 120 images per character) are already predefined.

## Used Architecture
Resnet18 

## Results
By using data augmentation, transfer learning and fine tuning, our model has reached a classification accuracy of 97% after only XX epochs. This result could be further improved by a little bit of additional effort. The first step would be to clean up the data set. Sometimes letters are so badly written that even humans might disagree about the classification.

## Installation Pytorch and Fastai

### Ubuntu / Kubuntu / Xubuntu / Lubuntu (Saucy and above)¶
#### pip
For detailed information please refer to https://github.com/fastai/fastai/blob/master/README.md#installation
     
     pip install fastai


Just make sure to pick the correct torch wheel url, according to the needed platform, python and CUDA version, which you will find at https://pytorch.org/get-started/locally/.

#### Proposed cloud platforms
https://www.paperspace.com<br>
https://colab.research.google.com

## Meta

Anel Music– [@LinkedIn](https://www.linkedin.com/in/anelmusic/) – anel.music@web.de

Distributed under the MIT license. See ``LICENSE`` for more information.

[https://github.com/AnelMusic/](https://github.com/AnelMusic/)

## Known Issues
Poorly written characters. Cleaning the dataset would result in a significant performance boost.

## Contributing

1. Fork it (<https://github.com/AnelMusic/Arabic_MNIST_Character_Classification//fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request

## Acknowledgements
I'd like to thank the researchers for providing the dataset.
Ahmed El-Sawy, Mohamed Loey, Hazem EL-Bakry, Arabic Handwritten Characters Recognition using Convolutional Neural Network, WSEAS, 2017
