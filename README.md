This file describes how run_analysis.R script works.

1.) unzip the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 
and rename the folder with "data".
Make sure the folder "data" and the run_analysis.R script are both in the current working directory.
2.) Source("run_analysis.R") command used.
3.) Two output files are generated in the current working directory would be found as follows:
merged_data.txt (7.9 Mb): it contains a data frame called cleanedData with 10299*68 dimension.
data_with_means.txt (220 Kb): it contains a data frame called result with 180*68 dimension.
4.) data <- read.table("data_with_means.txt") command in RStudio to read the file. 
Since we are required to get the average of each variable for each activity and each subject, 
and there are 6 activities in total and 30 subjects in total, we have 180 rows with all combinations 
for each of the 66 features.
