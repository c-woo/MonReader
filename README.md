# MonReader

I'll be attempting to create a deep learning model that can accurately classify whether or not a book page is being flipped in an image. 

Here's a quick look at some of the images from the dataset.

### Images
<img src='https://i.imgur.com/8rXriiq.jpg'>

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