# super-resolution-srcnn
Image Super-Resolution using Convolutional Neural Networks

# Prerequisites 
> keras with tensorflow

> opencv for python

> imutils

> scipy
    

## Steps to run
### 1-  Download the UKBench Dataset
- Go to the: [UKBench dataset](https://archive.org/download/ukbench)
- Download: ukbench.zip (Contains the raw .jpg images)

### 2- Add a data folder to the project
Following this structure: 
```
/data
    /input
        /ukbench00000.jpg	
        /ukbench00001.jpg	
        ...
    /ouput
```
### 3- Build a trainable dataset
```sh
$ python build_dataset.py
```
### 4- Train the super-resolution model
```sh
$ python train.py
```
### 5- Run the model on your own examples
```sh
$ python resize.py -i input_image.jpg -b baseline.jpg -o output_image.jpg
```
