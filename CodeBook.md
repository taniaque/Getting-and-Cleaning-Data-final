# Code Book
This code book will describe the data used in this project, as well as the processing required to create the resulting tidy data set.

## Overview
The smartphone captured various data about the movements volunteers wearing smartphone.

## Processing

+ All of the relevant data files were read into data frames, appropriate column headers were added, and the training and test sets were combined into a single data set.
+ All feature columns were removed that did not contain the exact string "mean()" or "std()".
+ The activity column was converted from a integer to a factor, using labels describing the activities.
+ A tidy data set was created containing the mean of each feature for each subject and each activity. Thus, subject #1 has 6 rows in the tidy data set (one row for each activity), and each row contains the mean value for each of the 66 features for that subject/activity combination. Since there are 30 subjects, there are a total of 180 rows.
