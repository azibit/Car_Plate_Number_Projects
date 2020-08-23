# Car_Plate_Number_Projects
An Object Detection project to detect plate numbers for cars in an image


## Creating a new Dataset

The following steps are needed to create a dataset for training and testing a Object Detection Model in MMDetection

## Step 1: Create the dataset folder structure

For this project, the files in the images directory are what we would be using to create the images in the train, test and valid dataset directory.

We put some images into the test2017 folder, some more images into the train2017 folder and some more into the val2017 folder.

We need to ensure that the data is in the COCO format, so we need to create the following folder structure

```
data 
	-> coco
	 	-> annotations
	 	-> test2017
	 	-> train2017
	 	-> val2017
```

We move 142 files from the images folder into the train2017, 20 files into the test2017 and also 20 files into the val2017 folder.



