## **Age Detection of Indian Actors**

This project employs deep learning techniques to classify Indian actors into three age groups: MIDDLE, YOUNG, and OLD. The dataset encompasses around 19,000 images, posing a challenge due to significant imbalance. We address this with label smoothing regularization and stratified K-fold cross-validation.

### **Dataset**

The dataset used for this project is publicly available on the [Analytics Vidhya website](https://datahack.analyticsvidhya.com/contest/practice-problem-age-detection/). It consists of images of Indian actors from different movies and TV shows, with ages ranging from 1 to 100 years old.

### **Model Architecture**

Several deep learning models were trained and tested for this project, including EfficientNet B2 and B3, ResNeXt50, and DenseNet121. The final model was created by ensembling the outputs of these models using the averaging technique.

### **Code**

The code for this project is written in Python using the PyTorch and scikit-learn libraries. The main files in the repository include:

- **`data_preprocessing.ipynb`**: Jupyter notebook containing code for preprocessing the data, including resizing the images, converting them to grayscale, and splitting the dataset into training and validation sets.
- **`train_models.ipynb`**: Jupyter notebook containing code for training the deep learning models using PyTorch, as well as the ensembling technique to create the final model.
- **`test_model.ipynb`**: Jupyter notebook containing code for testing the final model on the test dataset and generating the submission file.
- **`utils.py`**: Python script containing utility functions used in the project.

### **Results**

The final model achieved an accuracy of 92.7% and ranked 31 out of 8082 participants in the competition.

### **Conclusion**

This project demonstrates the use of deep learning techniques for age detection of Indian actors. The final model achieved high accuracy and can be used in real-world applications for automatic age detection in images and videos.
