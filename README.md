# Car_Plate_Number_Projects
An Object Detection project to detect plate numbers for cars in an image


## Creating a new Dataset

The following steps are needed to create a dataset for training and testing a Object Detection Model in MMDetection

## Section 1: Create the dataset folder structure

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

## Section 2: Create Annotation Files
Then we have a python script that combines each of the annotations for each folder into a single annotation file. The python script is titled labelme2coco.py

Run the labelme2coco.py for each of the train2017, test2017 and val2017 folders. Ensure labelme is installed before running the commands

For train2017
```
python labelme2coco.py train2017
```
It creates a file named trainval.json, rename the file as instances_train2017.json, then put the file in the annotations folder

For test2017
```
python labelme2coco.py test2017
```
It creates a file named trainval.json, rename the file as instances_test2017.json, then put the file in the annotations folder

For val2017
```
python labelme2coco.py val2017
```
It creates a file named trainval.json, rename the file as instances_val2017.json, then put the file in the annotations folder

## Section 3: Download and setup MMDetection
The framework MMDetection would be used for this project. We download MMDetection as follows:
```
git clone https://github.com/open-mmlab/mmdetection.git
```


