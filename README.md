# CSE-151B-kaggle-bot
## Large Files
The following files are in the dropbox folder because theya are too large for github. Please download them and place them in the data folder. (There is no folder in the github repo, just place all these files in the home repo as the jupyter notebooks.) Also, make sure to unzip the files before running the code. 
my_train_X; my_train_y; my_Y_train; my_Y_valid; my_y5_mlp_train; my_y5_mlp_valid.

dropbox link: https://www.dropbox.com/scl/fo/4xaw0ti3zw63as6vvyqx0/h?dl=0&rlkey=lsrbgn1yu5oh4f2zkdwor3x6d

## Google Drive
We also keep a copy of the data on google drive, the link is below. If any of the files in the dropbox cannot be open correctly, please try the google drive link and download the files with the same name. 

https://drive.google.com/drive/folders/1D_9pKgQSdpKuTPPXH6duxz3vAVviT22P?usp=sharing

## Usage Instructions
### General
Given the current files in the github and dropbox, you should be able to run the 5th jupyter notebook file named just run without trainning anything. All of the models and data has been created. You can just run the code and it will output the predictions. However, if you want to try to run something else like machine learning algorithms or different models, you can run the other jupyter notebook files. The order is from first to last. 

### 5th File: Just Run
Like we said above, you can run this file and generate the final combined model with MLP output (the 320 rows test file) without training anything. This is the best model we submitted to kaggle. 

### 1st File: Data Processing
This file will process the raw training data using multiple strategies. It will output the processed one-hot encoded data with 589 columns. The output file is in csv format. 

### 2nd File: Model Training
This file will fit all the machine learning algorithms as well as the initial MLP that passes in the dataset with 589 columns. The output will be a new dataset with 5 columns. Each column is the prediction of the corresponding model. It will also output the files of all five models.

### 3rd File: Given Models
This file will be given all fitted models, and print the loss of each model. This is basically 2nd file without the training part.

### 4th File: Combining models
Given the dataset with 5 columns, this file will fit the linear regression model to combine the predictions of the 5 models. It will output the combined prediction. It will also train in the combine MLP model to generate the ultimate prediction of the public test set. This file is basically the 5th file with the training part. 

__Note:__ Please have lightGMB installed in your environment. If not, use ``conda install lightgbm`` in conda environment or ``pip install lightgbm`` in virtual environment. 
Please have scokit plot installed in your environment. If not, use ``conda install scikit-plot`` in conda environment or ``pip install scikit-plot`` in virtual environment.
Please have seaborn installed in your environment. If not, use ``conda install seaborn`` in conda environment or ``pip install seaborn`` in virtual environment.


