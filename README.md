# Cornell Birdcall Identification
140th Place Solution to Kaggle competition Cornell BirdCall Identification  
  
The idea is that sound file can be converted to an "image" format and use the usual techquies of visual recognition to train and predict on the bird sound dataset.

By melspectrogram function, sound files can be converted into a 2D matrix, the x-axis is time and y-axis is the frequency. The values of the matrix represents the intensity of the sound recorded of a particular frequency at a particular time.  
  
The 2D matrix being transformed can be viewed as a 2D mono image. By stacking up the 2D mono image into 3 color channels, the output can be put into the ResNet.  
  
Usual techquies of augmenting the picture can be applied, particularly croping and random rotation is used to improve resilience of the model. 

For the model files used in this solution, please find in https://www.kaggle.com/hsfert/birdsong-resnet101/.