This code book summarizes the steps or process to get to the results included in tidy.txt.

Steps
The run_analysis.R file performs five steps listed in the course project:
1. First, workind directory was set up in the location where dataset was downloaded and unzipped.
Activity labels and features were read using appropriate codes. 
  Following activity labels were observed:
•	WALKING: subject was walking during the test
•	WALKING_UPSTAIRS: subject was walking up a staircase during the test
•	WALKING_DOWNSTAIRS: subject was walking down a staircase during the test
•	SITTING: subject was sitting during the test
•	STANDING: subject was standing during the test
•	LAYING: subject was laying down during the test
2. Data on mean and standard deviation were extracted in the second step. 
3. Training and test dataset were uploaded (read in R)
4. All the similar data is merged (merged_data object) using the rbind() function and given the correct names. By similar, I mean the files having the same number of columns and referring to the same entities.
5. Activity and subject were turned into factor.  	
6. As activity data is addressed with values 1:6, we take the activity names and IDs from activity_labels.txt and they are substituted in the dataset.
7. Finally a new dataset (tidy.txt) with all the average measures for each subject and activity type (30 subjects * 6 activities = 180 rows) was generated. The output file is uploaded in the repository. 
