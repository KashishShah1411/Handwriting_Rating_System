# Handwriting_Rating_System
Handwriting Rating System using **Convolution Neural Networks** and some concepts of low level **Computer Vision**. We use a combination of MNIST and Kaggle A-Z datasets for the model building and training it for Character Recognition. We applied **Contour Detection using Canny Edge Detection** on the test image to find the contour of a particular character predicted by the model. 
We created CNN classification model of our own using the datasets.

For classification of Good and Bad Handwriting, we first saved the contours of good hand-written characters and then used them to compare with the predicted contours of test images. We used **Structural Similarity Index Metric**.

### Installation
For Google Collab, you need to just import the libraries/datasets used. For example, for importing MNIST dataset, 
```
from tensorflow.keras.datasets import mnist
```
Similarly, for importing libraries,
```
import numpy as np
```
For Jupyter Notebook or any other environment, user needs to install the following libraries, 
```
TensorFLow
Keras
Numpy
Pandas
SciKitImage
cv2
os  
matplotlib
imutils
``` 
### Running the tests
Download the [dataset](https://www.kaggle.com/sachinpatel21/az-handwritten-alphabets-in-csv-format) from Kaggle. Upload the path of the dataset in the environment being used. 

Upload the hand written image for which the classification needs to be done, on the environment. For every character, the user will get the  characteristics.

### Other Attempts
- We also tried another approach :
We created another model and trained it with data of good handwritting characters. After training we predicted the output using both the models i.e the precious model which was trained with mnist and kaggle a-z dataset.

We will classify the handwritting as good or bad based upon how the output from the previous model is similar to the output of model which is created with the good handwritting characters dataset.

If a character is badly written then the new model will not recognize it as it is trained with good training set
but the old model would have recognized it so the user has to improve writting for that character
This approach will generate better results as we are comparing results with the best set. But as we were not having a large dataset of good handwritting characters the model which was generated was not able to generalise well


### Built With

- Python 

### Contributors

- [Kashsish Shah](github.com/KashishShah1411)
- [Harsh Patel](github.com/hap662000)
- [Hriday Nagrani](github.com/HridayNagrani)
- [Dhruv Shah](github.com/dhruvshah01)

Youtube Video Link: https://www.youtube.com/watch?v=WKeA4-MTOlk
