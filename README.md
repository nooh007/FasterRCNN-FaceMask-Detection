Faster R-CNN Implementation in Pytorch

This repository implements Faster R-CNN with Resnet-50 Backbones in Pytorch.

This faster RCNN implementation can be used for any custom dataset, and make sure to follow the steps from the Tutorial to avoid any errors.


## Sample Output by training Faster R-CNN on FaceMask dataset 
Ground Truth | Prediction
</br>
<img src="https://github.com/user-attachments/assets/da09d1fa-f013-4150-9457-d6396d19ebe0" width="300">
<img src="https://github.com/user-attachments/assets/7c2c7de7-8fc3-4d1d-aa9c-268d5410961f" width="300">
</br>
<img src="https://github.com/user-attachments/assets/e45ff977-c102-4824-86dc-6a6247456121" width="300">
<img src="https://github.com/user-attachments/assets/df8673b1-ec17-4110-919e-0ca9c0934b9d" width="300">

## Data preparation

Please ensure that when downloading the dataset in Pascal VOC format, you place the training and testing images in their respective JPEGImages folders, and similarly, store the corresponding annotations in the Annotations folders for training and testing separately.
The Tree structure of the directory should look like the following.
FasterRCNN-Pytorch
```
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






## References

- Implementation inspired by the [FasterRCNN-PyTorch repository by explainingai-code](https://github.com/explainingai-code/FasterRCNN-PyTorch).

