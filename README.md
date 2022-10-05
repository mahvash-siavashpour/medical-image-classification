# medical-image-classification
In this project a medical image classification task was implemented using a convolutional neural network with different layers stack on top of each other.

## Data set
Adapted version of Paul Mooney's 'Chest X-Ray Images (Pneumonia)' dataset. <br>
Total number of observations (images): 5,856 <br>
Training observations: 4,192 (1,082 normal cases, 3,110 lung opacity cases) <br>
Validation observations: 1,040 (267 normal cases, 773 lung opacity cases) <br>
Testing observations: 624 (234 normal cases, 390 lung opacity cases) <br>
(source: [Kaggle](https://www.kaggle.com/datasets/pcbreviglieri/pneumonia-xray-images)) <br>

![data](https://github.com/mahvash-siavashpour/medical-image-classification/blob/main/x-ray.png?raw=true)

## Model Description
For the purpose of designing a model capable of learning to categorize x-ray images in one of the NORMAL or PNEUMONIA a convolutional neural network was obtained. The CNN consists of 5 convolutional layers each followed by a maxpooling layer. the ouput of these convolutional in then flatten and fed into a fully connected neural network and finaly classified using a single neuron with sigmoid activation function. A binary crossentropy loss function and adam optimizer was used to train this model on 5 epochs. After the training an accuracy of 97% was obtained on the test dataset. <br>

## Results
The digram of the training process in the 5 epochs is depicted below:<br>
![training digram](https://github.com/mahvash-siavashpour/medical-image-classification/blob/main/history.png?raw=true)

The in-depth summary of the metrics is as follow: <br>
![result](https://github.com/mahvash-siavashpour/medical-image-classification/blob/main/result.png?raw=true)
