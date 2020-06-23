# EEG-Visualization
Data Visualization of EEG signals. This project consists dataset description, data pre-processing and data visualization.

# Dataset description:
This data arises from a large study to examine EEG correlates of genetic predisposition to alcoholism. It contains measurements from 64 electrodes placed on the scalp sampled at 256 Hz.

There are 3 parts of dataset available for experiment purposes.
1. The small dataset: Only 2 subjects. Alcoholic and Control each.
2. The large dataset: Total 20 subjects. Alcoholic and Control subjects each 10.
3. The full dataset: Total 120 subjects consisting of Alcoholic and Contorl group.

Here, we will use The large dataset for learning purpose with data of 20 subjects in total. 

Data Collection process:
* In the data collection, two grouped were created - Alcoholic (10 subjects) and Control (10 subjects). 
* Each subject was connceted with 64 sensors. Here, sensors are mentioned as Channel. 
* Each subject was exposed to either a single stimulus (S1) or to two stimuli (S1 and S2) which were pictures of objects chosen from the 1980 Snodgrass and Vanderwart picture set. When two stimuli were shown, they were presented in either a matched condition where S1 was identical to S2 or in a non-matched condition where S1 differed from S2. 
* For every stimuli of each trial records voltage of all channels for one second time period. 
* The frequency of recording by each channel is 256 datapoints per second. These data frequency is mentioned as epochs. 
* The next column is alchohoilc. It is a boolean data. True defines the subject is from alcoholic group, false denies the subject is from control group. 
* The final column is subject_id. Subject ID is unique ID assigned to each subject. It is an alphanumeric datatype. 4th letter of this alphanumeric data is either 'c' or 'a'. From here also, we can find if the subject is from alcoholic group or control group. 'a' = alcoholic, 'c' = control.

The dataset is in compressed file format. To decompress the data and create dataframe from it, is describe in the data_preprocessing notebook.
