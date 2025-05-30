Faster R-CNN Implementation in Pytorch

This repository implements Faster R-CNN with training, inference and map evaluation in PyTorch.
The aim was to create a simple implementation based on PyTorch faster r-cnn codebase and to get rid of all the abstractions and make the implementation easy to understand.

Here i have used the Facemask dataset from kaggle to perform the implementation.

This faster RCNN implementation can be used for any custom dataset, and to make sure to follow the steps from the pdf to avoid any errors.


## Sample Output by training Faster R-CNN on FaceMask dataset 
Ground Truth(Left) | Prediction(right)
</br>
<img src="https://github.com/user-attachments/assets/da09d1fa-f013-4150-9457-d6396d19ebe0" width="300">
<img src="https://github.com/user-attachments/assets/e45ff977-c102-4824-86dc-6a6247456121" width="300">
</br>
<img src="https://github.com/user-attachments/assets/7c2c7de7-8fc3-4d1d-aa9c-268d5410961f" width="300">
<img src="https://github.com/user-attachments/assets/df8673b1-ec17-4110-919e-0ca9c0934b9d" width="300">

## Data preparation
For setting up the VOC 2007 dataset:
* Download VOC 2007 train/val data from http://host.robots.ox.ac.uk/pascal/VOC/voc2007 and name it as `VOC2007` folder
* Download VOC 2007 test data from http://host.robots.ox.ac.uk/pascal/VOC/voc2007 and name it as `VOC2007-test` folder
* Place both the directories inside the root folder of repo according to below structure
    ```
    FasterRCNN-Pytorch
        -> VOC2007
            -> JPEGImages
            -> Annotations
        -> VOC2007-test
            -> JPEGImages
            -> Annotations
        -> tools
            -> train.py
            -> infer.py
            -> train_torchvision_frcnn.py
            -> infer_torchvision_frcnn.py
        -> config
            -> voc.yaml
        -> model
            -> faster_rcnn.py
        -> dataset
            -> voc.py
    ```

## For training on your own dataset



## References

