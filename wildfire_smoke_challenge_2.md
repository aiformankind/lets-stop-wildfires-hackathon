# Challenge II: Start of Smoke Ignition

We launched this Wildfire Smoke Detection Challenge in conjunction of the **Let’s Stop Wildfires Hackathon**. In this challenge, you task is to build an early wildfire smoke detector. We provide the following HPWREN camera image sequences as training dataset. You can use your solution as the entry to the Let's Stop Wildfire Hackathon. The same hackathon rules apply to this challenge. See [rules](README.md)

#### Train Dataset
You can download the train dataset here. It consists of multiple subfolders. Each subfolder contains the image sequences captured by a HPWREN camera when a fire broke out. Since the goal is to early detect the wildfire, these sequences consist of images ~40 mins before and after the ignition of fire. The images are time ordered.  Open the provided label_meta.csv to find out the first image in the sequence that has the first appearance of smoke.

[train dataset](https://tinyurl.com/yy3evlfx)

[label_meta.csv](https://tinyurl.com/y2g2o2jk)

#### Submission
You will have to create a new github repo for your codes with the MIT License. See Hackathon rules for more infos. For evaluation, we will run your program against a new test dataset. The test dataset will have the same directory structure as the train dataset.

You need to build a model that uses previous last seen image sequences (moving window) to predict the presence of smoke in the current image.  
Your program will read a folder consists of multiple subfolders where each subfolder contains image sequences captured ~40 mins before and after the first fire ignition. In the end, your program will output a CSV with the following format.

##### Output File
folder_name, smoke_detected(yes/no), image_filename_where_smoke_detected, index of image in the sequence (zero indexed, -1 if no smoke detected)

Example:
```
20170625-BBM-bm-n-mobo,yes,1498416633_+00240.jpg,14
20170625-BBM-wk-w-abbc,no,-,-1
```
Note: 
If no smoke detected in the sequence, use -1 as index of image and use - in the image name column.

#### Contact Us
Please feel free to reach out to us if you have any questions. Join AI For Mankind **Slack** [https://tinyurl.com/y6pvbwee](https://tinyurl.com/y6pvbwee) channel to ask question.
