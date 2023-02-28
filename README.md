Age Detection of Indian Actors
This repository contains the code for my Age Detection of Indian Actors project, which is a deep learning model that classifies Indian actors into three age groups: MIDDLE, YOUNG, and OLD. The dataset consists of approximately 19,000 images, which were highly imbalanced. To handle this, I used label smoothing regularization and stratified K-fold cross-validation techniques.

I trained multiple models, including EfficientNet_B2, B3, ResNeXt50, and DenseNet121. I then combined them using an ensembling averaging technique to improve the overall accuracy of the model. The final model achieved an accuracy of 92.7% and ranked 31 out of 8082 participants in the competition.

Requirements
Python 3.6+
PyTorch 1.6+
torchvision 0.7+
scikit-learn 0.23+
Installation
Clone this repository.

Install the required packages using the following command:

Copy code
pip install -r requirements.txt
Usage
To train the model, run the following command:

css
Copy code
python train.py --data_path path/to/dataset --save_path path/to/save/model
You can specify the hyperparameters for training using the command line arguments, or modify them in the config.yaml file.

To evaluate the model on the test set, run the following command:

css
Copy code
python evaluate.py --data_path path/to/test/dataset --model_path path/to/saved/model
This will output the accuracy and F1 score for the model.

Results
The final model achieved an accuracy of 92.7% on the test set and ranked 31 out of 8082 participants in the competition.

License
This project is licensed under the MIT License - see the LICENSE.md file for details.

Acknowledgments
The dataset for this project was provided by Analytics Vidhya.
The code for this project was inspired by the PyTorch template from cs230-stanford.


