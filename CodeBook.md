# Instructions

1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement.
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive variable names.
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

# Datasets

- 'features_info.txt': Shows information about the variables used on the feature vector.
- 'features.txt': List of all features.
- 'activity_labels.txt': Links the class labels with their activity name.
- 'train/X_train.txt': Training set.
- 'train/y_train.txt': Training labels.
- 'test/X_test.txt': Test set.
- 'test/y_test.txt': Test labels.

# Variables

- x_train         Memory Table for training set data
- y_train         Memory Table for training labels data
- subject_train   Memory Table for training subject data
- x_test          Memory Table for testing set data
- y_test          Memory Table for testing labels data
- subject_test    Memory Table for testing subject data
- features        Memory Table of correct names for x_data
- activities      Memory Table for activities labels data
- x_data          Merges x_train & x_test datasets
- y_data          Merges y_train & y_test datasets
- subject_data    Merges subject_train & subject_test datasets
- all_data        Merges x_data, y_data and subject_data
- averages        Contains the averages required whic are stores in averages.txt file

# Adds

ddply() from the plyr package is used to apply colMeans() and simplify the code.
