Faster R-CNN Implementation in Pytorch

This repository implements Faster R-CNN with training, inference and map evaluation in PyTorch.
The aim was to create a simple implementation based on PyTorch faster r-cnn codebase and to get rid of all the abstractions and make the implementation easy to understand.

Here i have used the Facemask dataset from kaggle to perform the implementation.

This faster RCNN implementation can be used for any custom dataset, and to make sure to follow the steps from the pdf to avoid any errors.


## Sample Output by training Faster R-CNN on FaceMask dataset 
Ground Truth(Left) | Prediction(right)
</br>
<img src="https://github.com/explainingai-code/FasterRCNN-PyTorch/assets/144267687/d9e8bfbb-d6c3-4cb7-955f-e401ebb9045c" width="300">
<img src="https://github.com/explainingai-code/FasterRCNN-PyTorch/assets/144267687/2fe01174-dd0d-4fee-afbd-45b5b45307b3" width="300">
</br>
<img src="https://github.com/explainingai-code/FasterRCNN-PyTorch/assets/144267687/39f095d3-8f50-4cd7-89cb-cee655cfa76d" width="300">
<img src="https://github.com/explainingai-code/FasterRCNN-PyTorch/assets/144267687/2860bb29-3691-419a-b436-0d67f08d82e0" width="300">

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

