# Mushroom Classification: Edible or Poisonous

This project aims to develop machine learning and deep learning models to accurately classify mushroom images into edible or poisonous categories. The challenge lies in the large number of mushroom species and their diverse visual characteristics, which make visual identification difficult. The project also aims to compare the performance of various models within the constraints of a limited number of available images.

## Dataset
The dataset used in this project, obtained from Kaggle, comprises over 3000 images of mushrooms. Among these, 1181 images are classified as edible, while 2220 images are labeled as poisonous. The images in the dataset have varying sizes, with most of them being around 250x250 pixels.

## Methods
We propose the use of three machine learning methods for classifying the mushroom images: Random Forest, Kernel Support Vector Machines (Kernel SVM), and Convolutional Neural Networks (CNN). For the CNN, we leveraged transfer learning, specifically using the pre-trained ResNet50 model.

## Results
The Random Forest algorithm demonstrated high accuracy on the training set, achieving a perfect fit. After optimizing its hyperparameters, we achieved an accuracy of 0.648 on the testing set.

The Kernel SVM algorithm achieved an accuracy of 0.656 on the testing set. Although it had high accuracy on the training set (0.940), there is room for improvement in accurately predicting the 'edible' class.

The CNN without transfer learning achieved moderate accuracy on the testing set. However, there was a noticeable gap between the training and validation accuracies, suggesting potential overfitting.

In contrast, the Transfer Learning approach using the ResNet50 model did not yield satisfactory results. The model struggled to learn meaningful patterns and achieve accurate predictions.

## Conclusion
Overall, the Random Forest algorithm exhibited the most promising results in terms of accuracy, precision, recall, F1-scores, and discriminatory power. However, further analysis and improvement are required for the Transfer Learning approach to enhance its classification accuracy and performance.

## References
The dataset used in this project can be found [here](https://www.kaggle.com/datasets/marcosvolpato/edible-and-poisonous-fungi).
