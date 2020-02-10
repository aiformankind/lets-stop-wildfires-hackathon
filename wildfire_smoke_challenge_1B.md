# Challenge IB: Smoke vs No Smoke using Gridded Image

In this challenge, every HPWREN captured image is cut into multiple small grids. 
Your task is to build a wildfire smoke classifier to predict if there is smoke given a 
small grid image.
 
You can use your solution as the entry to the Let's Stop Wildfire Hackathon. 
The same hackathon rules apply to this challenge. See [rules](README.md)

#### Train Dataset
You can download the train dataset below. 
It consists of two folders, one contains smoke and the other contains no_smoke grid images. 

You can download the train dataset from below Dropbox link.

* [Dropbox: train dataset](https://www.dropbox.com/s/5rue8c28iidvlvh/grid_smoke_version.tar)


#### Submission
You will have to create a new github repo for your codes with the MIT License. To allow us to evaluate your model against our test dataset, you can either 

1) Save your model in HDF5 format and share it in your repo. If the model size is over 100MB, please provide either Dropbox or Google Drive link to your model. We will load your model and evaluate it against our test dataset.

or

2) Provide a python program to read in a folder consists of multiple images and predict whether there is smoke or no smoke in each image and write the output in a CSV file with the following format.


##### Output File
image_name, smoke_detected(1 if smoke detected or 0 if no smoke)

Example:
```
image_name_a,1
image_name_b,0
```

#### Contact Us
Please feel free to reach out to us if you have any questions. Join AI For Mankind **Slack** [https://tinyurl.com/rrsflyv](https://tinyurl.com/rrsflyv) channel to ask question.
