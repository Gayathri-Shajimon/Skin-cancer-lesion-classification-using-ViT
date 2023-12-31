# Skin-cancer-lesion-classification-using-Vision-Transformer

## Execution Instructions

Step 1 : Download the train, validation and test dataset from ISIC 2017 archive - https://challenge.isic-archive.com/data/#2017

## Using the augument_it.ipynb script

Step 2a : The script reads ground truth information from CSV files using Pandas DataFrames within each of the downloaded data archives.

Step 2b : The `resize_images_in_folder()` function resizes images in the train, test, and validation directories.

Step 2c : The `task1_spliter()` and `task2_spliter()` functions split data for Task 1 and Task 2 into separate folders based on labels.

Step 2d : New directories are created for each task type (melanoma, nevus, seborrheic keratosis) in the train, test, and validation directories.

Step 2e : Images are copied to the corresponding task-specific directories.

Step 2f:  Training and validation data are merged into a "train_merged" directory for cross-validation purposes.

Step 3 : Train the model using the corresponding data.

Note: The script assumes that image files follow the ".jpg" or ".jpeg" format and are stored in the specified paths. Files with other formats will be skipped during the resizing and copying process.

For data augmentation, the script generates and saves images to disk. Images generated for each task are six times their original size.


Within this set of data folders, you'll find the following:

### `train`

The `train` folder contains the competition's training data. These images are crucial for training machine learning models.

### `val`

In the `val` folder, you'll discover the competition's validation data. These images play a pivotal role in fine-tuning models during the validation stages.

### `test`

The `test` folder houses the competition's testing data. These images are designed for evaluating model performance on previously unseen data.

### `train_merged`

The `train_merged` folder is a combined repository of both the training and validation data. This combination serves to facilitate cross-validation procedures.

### `train_augmented`

Within this folder, you'll find a fusion of the original images from the `train` folder and additional augmented images used for training purposes.

### `train_merged_augmented`

Similar to the `train_augmented` folder, `train_merged_augmented` contains augmented images combined with the original images from the `train_merged` folder.



## Repostory Structure

Final Code - is the main folder which contains all the folders associated with the project
The final code contains 4 folders –
•	Exploratory Data Analysis – This contains all the exploratory data analysis done and displayed in the report.

•	Data Handling - This folder contains the resizing and categorizing of the images into folders. A detailed explanation data handling folder is there in the data Handling folder itself.

•	Train + Test – is setting S1 in the report, Cross-validation is SS1 and Normal Train and Test is SS2 in the report (Section 3.10)

•	Train + Validation + Test - is setting S2 in the report, Cross-validation is SS1 and Normal Train and Test is SS2 in the report (Section 3.10)


![image](https://github.com/Gayathri-Shajimon/Skin-cancer-lesion-classification-using-Vision-Transformer/assets/149523953/00b234aa-15a4-4ba9-80ba-62e90e1272de)

