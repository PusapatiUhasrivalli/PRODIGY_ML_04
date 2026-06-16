# Hand Gesture Recognition using SVM

## Overview
This project implements a Hand Gesture Recognition system using a Support Vector Machine (SVM) classifier. The model is trained to classify different hand gestures from image data and demonstrates high classification accuracy.

## Dataset
- Dataset: Hand Gesture Recognition Dataset
- Number of Classes: 20
- Images per Class Used: 100
- Total Images Used: 2000

## Technologies Used
- Python
- OpenCV
- NumPy
- Scikit-learn
- Google Colab

## Methodology
1. Extract and load the dataset.
2. Resize images to 64×64 pixels.
3. Convert images into flattened feature vectors.
4. Assign labels based on gesture classes.
5. Split the dataset into training and testing sets (80:20).
6. Train a Linear Support Vector Machine (SVM) classifier.
7. Evaluate model performance using classification metrics.

## Model Training

python
from sklearn.svm import SVC

svm_model = SVC(kernel='linear')
svm_model.fit(X_train, y_train)


## Results

| Metric | Score |
|----------|----------|
| Accuracy | 99.75% |
| Precision | 99.8% |
| Recall | 99.8% |
| F1-Score | 99.8% |

## Conclusion

A Support Vector Machine (SVM) classifier was developed for Hand Gesture Recognition using a dataset containing 20 gesture classes. The images were resized to 64×64 pixels and converted into feature vectors using flattened pixel values.

The dataset was split into training and testing sets in an 80:20 ratio. A Linear SVM model was trained on the training data and evaluated on the testing data.

The model achieved *99.75% accuracy*, demonstrating excellent performance in recognizing and classifying hand gestures. These results show that SVM can be highly effective for image-based gesture recognition tasks when combined with appropriate preprocessing techniques.
