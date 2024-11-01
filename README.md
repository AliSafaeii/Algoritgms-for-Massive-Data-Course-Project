This project is aimed at designing and implementing an image classifier that can recognize pictures
within a subset of the Prado Museum Pictures dataset (an available dataset on the Kaggle website).
The project dataset is classified based on the four most frequent techniques used in the artworks in the
Prado Museum Pictures dataset. These techniques include oil painting, coinage, sculpture and
composite pencil. Three different models using convolutional neural networks have been introduced,
and their performances have been analysed. All the models are based on transfer learning, utilizing
three different pre-trained feature extractors.
From a high-level perspective, each model consists of a pre-trained feature extractor followed by a
fully connected layer with 128 neurons, and then a softmax layer. Dropout and data augmentation
techniques, which can be helpful to prevent overfitting, are employed. The pre-trained feature
extractors are based on the VGG16, ResNet50 and InceptionV3 models, which have been previously
trained on the ImageNet dataset. Among the models, the one using the pre-trained feature extractor
based on InceptionV3 outperformed the others, achieving an 98.57% accuracy on the test set.
