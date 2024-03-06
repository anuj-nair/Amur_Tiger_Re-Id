## Amur Tiger Re-ID

Inspired by [Tiger Ident F1 score=98%](https://www.kaggle.com/code/gpiosenka/tiger-ident-f1-score-98)

### Tiger Re-ID Data Prep
- Downloaded data from [Amur Tiger Re-Identification](https://www.kaggle.com/datasets/quadeer15sh/amur-tiger-reidentification).
- Loaded the data and splitted it to train, validation and test dataset.
- Found mean and standard deviation for each RGB values for entire training set.
- It is used for image data normalization.
- Due to limited amount of training data, we create 150 image per class  using data augmentation.
- Resized all image to  300x300 and normalized the  images before storing them.

### Tiger Re-ID
- Created custom dataset and loaded the data.
- Created a model using transfer learning.
- Used ResNet model as base and  added 2 more full connected layers. 
- Trained and validated the model on training and validation dataset.
- Finally tested the accuracy in test dataset with 92.3%.


