## **Age Detection of Indian Actors**

This project employs deep learning techniques to classify Indian actors into three age groups: MIDDLE, YOUNG, and OLD. The dataset encompasses around 19,000 images, posing a challenge due to significant imbalance. We address this with label smoothing regularization and stratified K-fold cross-validation.

### **Dataset**

The dataset is publicly available on the **[Analytics Vidhya website](https://datahack.analyticsvidhya.com/contest/practice-problem-age-detection/)**. It spans images of Indian actors across movies and TV shows, depicting ages from 1 to 100 years old.

### **Model Architecture**

Multiple deep learning models were employed, including EfficientNet B2 and B3, ResNeXt50, and DenseNet121. We finalized the model through ensembling these models' outputs using averaging.

### **Code**

Our code, implemented in Python using PyTorch and scikit-learn, is organized into key files:

- **`data_preprocessing.ipynb`**: Jupyter notebook for preprocessing, including resizing, grayscale conversion, and dataset division.
- **`train_models.ipynb`**: Jupyter notebook to train models using PyTorch and apply ensembling.
- **`test_model.ipynb`**: Jupyter notebook for testing the final model and generating submissions.
- **`utils.py`**: Python script with utility functions.

### **Results**

The model achieved 92.7% accuracy, securing the 31st position out of 8082 participants in the competition.

### **Conclusion**

This project showcases effective deep learning techniques for age detection in Indian actors. The high-performing model holds potential for real-world image and video applications, automating age detection with precision.
