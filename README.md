# Classification and identification of ships.
This Dataset is taken from Deep Learning Hackathon organised by Analytics Vidhya.
can be found here https://www.kaggle.com/datasets/arpitjain007/game-of-deep-learning-ship-datasets
![tif134](https://user-images.githubusercontent.com/77253306/172779838-4a206beb-6b70-441a-8bb6-cf2ee9b07b5c.png)

# Summary
The detection of objects in images and video allows tasks to be carried out automatically as computers are capable of recognizing objects from an image and making decisions.

![tif23](https://user-images.githubusercontent.com/77253306/172938036-e2541e88-83d2-4733-b49e-56f1e4c7533a.png)

YOLO (You Only Look Once) is a system that uses classifiers to perform object detection. Applying a classification model to an image in multiple locations and scales, where the regions obtain a high score are considered detections.


# Training
In order to make use of the convolutional neural network for object detection training, the repository where the model is located and the pre-trained weights for this model are cloned.

### YOLO V4 pre-trained model repository cloning
![image](https://user-images.githubusercontent.com/77253306/172941161-67c900ed-8138-4a56-a266-b5236e62c78b.png)

### Download of pre-trained weights of YOLO V4 model.

![image](https://user-images.githubusercontent.com/77253306/172941945-9ae09ec7-ee2f-42d8-8317-0dbfa309f676.png)

Once the model and the pre-trained weights have been downloaded, the directories containing the training, validation and test images are loaded.

### Loading images used in training

![image](https://user-images.githubusercontent.com/77253306/172942371-35339d80-41c0-4098-8d6f-d450d5c0d974.png)


The training carried out for the detection of 5 different classes of ships was carried out with 200 images per class, with a total of 1000 training images. However, they were divided into 80% for training, 15% for validation, and 5% for testing. 

The training lasted 3:30 hours, because the performance did not increase appreciably at this point and because it was possible to stop the training since the training data was autosaved.

# Results
The mAP (mean average precision) for each class exceeded 90% except for the cargo class and the IoU reached 71.51% using a threshold of 50%.

![tif34](https://user-images.githubusercontent.com/77253306/172780481-b48d0366-a90a-46a3-b5f4-ab4ebe6a3fe2.png)

Predictions made with the test set.

![image](https://user-images.githubusercontent.com/77253306/172944363-13a6c72d-6bb7-4e61-a6e8-669f36e9b9ab.png)

