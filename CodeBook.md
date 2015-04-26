Method to process the data
------------------------------------
Fist I read the data from the files and store them in test and train files and then combine the test and train data using the row binding function.
Then, only columns with mean and standard deviation measures are taken from the whole dataset. 
As activity data is addressed with values 1:6, is taken from activity_labels.txt and they are replaced in the dataset.
Column names are corrected.
Then I generate a new dataset with all the average measures for each subject and activity type. The output file is called averages_data.txt, and uploaded to this repository.
Variables in the script
----------------------------
x_train, y_train, x_test, y_test, subject_train and subject_test contain the data from the downloaded files.
x_data, y_data and subject_data merge the previous datasets to further analysis.
features contains the correct names for the x_data dataset, which are applied to the column names stored in mean_and_std_features, a numeric vector used to extract the desired data.
all_data merges x_data, y_data and subject_data in a big dataset.
Finally, averages_data contains the relevant averages which will be later stored in a .txt file. 
