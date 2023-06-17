# safety_helmet_detector-by-yolov8
  This is a project trying to detect the safety-helmet by using Yolov8.
## Model 1: 50 imgs
  Since this model is absolutely overfitting, I would just show the confusion matrix in the following. This is just a beta model to experience the process of a cv detection work. For the labeling step, I just simply use the cvat.ai.
  
  The confusion matrix is like the following picture:
  ![image](model50/results/confusion_matrix_normalized.png)
  

## Model 1: 1700 imgs
  ### Dataset
  - website : https://www.kaggle.com/datasets/vodan37/yolo-helmethead (which has two types of label, one is safety_helmet, another one is simply just head (without safety_helmet))
  - data selection: I just literally simplified the natural 20000+ imgs to 1700 pics, and use 300 pics as the validation set.

  ### Model Selection
  - The official yolo v8 website offered plenty of models to select, however, in this project, I just used yolov8-nano (20 epochs, 50 epochs, 100epochs), yolov8-nano-pretrained (50 epochs) and yolov8-small-pretrained (50 epochs) as the training model (totally 5 models).
  - official docs website of yolov8: https://docs.ultralytics.com/

  ### Envs.
  - Autodl platform with a single RTX-3080, the envs is Pytorch 1.10.0, python 3.8(ubuntu20.04)

  ### Training Process:
  - yolov8-nano, 20 epochs
    - Confusion Matrix(Normalized):
      
  - yolov8-nano, 50 epochs
    
  - yolov8-nano, 100 epochs
    
  - yolov8-nano-pretrained, 50 epochs
    
  - yolov8-small-pretrained, 50 epochs
  
  
