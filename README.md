# MonReader

A mobile digital documentation app used for automatic, quick, and high quality document scanning requires the app to know whether or not a page is being flipped in order to take pictures correctly. The app needs to be able to take pictures while a page is still and not being flipped in order to take high quality pictures of each page. If the app cannot distinguish if a page is being moved, it might take pictures while there is movement, causing the images to be low quality and unusable rendering the app useless.

I'll be attempting to create a deep learning model that can accurately classify whether or not a book page is being flipped in an image.

### Images
Here's a quick look at some of the images from the dataset.

<img src='https://i.imgur.com/LZN4lXx.jpg'>

### Image Augmentation
'''
img_augmentation = models.Sequential(
    [
        layers.RandomRotation(factor=0.15),
        layers.RandomFlip()
    ])
'''

<img src='https://i.imgur.com/l7YMLEk.jpg'>


## Models Used for Predictions

The best performing models were ones made with Transfer Learning. 

The models I tested are:<br>
* ResNet-50
* EfficientNet

## ResNet-50
<img src='https://i.imgur.com/1zdGMoL.jpg'>

### Evaluation Metrics
Accuracy: 97.99%<br>
Precision: 96.53%<br>
Recall: 99.67%<br>
F1-score: 98.08%<br>

## EfficientNet
<img src='https://i.imgur.com/g0QaJX1.jpg'>

### Evaluation Metrics
Accuracy: 97.32%<br>
Precision: 96.19%<br>
Recall: 98.70%<br>
F1-score: 97.43%<br>


## Conclusion
Both ResNet and EfficientNet performed extremely well in predicting whether or not a page is being flipped. Transfer Learning with ResNet does perform slightly better than using EfficientNet with an accuracy score of 98% and a F1-score of 98%.


z2EMbf1cjGmX8MSU