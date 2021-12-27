# Siamese_SSD_Based_CV_Counter

An AI based computer vision counter that detects, classifies and counts objects according to their respective classes with near realtime latency.

## Progress after YOLO based Counter:
This model is based on the developments suggested within my undergrad internship report (**YOLO_Based_Model_Internship_Report_**). This model works on improvements in accessibility and scalability that the YOLO based Counter lacked. In this model, the single stage object detection-classification based on YOLO V3 is replaced with two staged object detection (**SSD MobileNetV2**) and classification (**Resnet50 based Siamese Neural Network**). The seperation of tasks in the updated counter allows users with greater control on where to classify the detected objects in the screen depending on where the view of the object is best. This would potentially allow lower need for training images for industrial production given enough volume of data is used to train the Siamese NN backbone priorly.

**Siamese_Make_Trials_Fin**: Notebook with codes on training the Siamese NN backbone.
**SNN_RnD_Project_Script**: Notebook consisting of codes to run the counter on video.
**testing_videos**: Directory consisting of videos that can be used to run demo counting with pretrained model.
**imageacc_model.h5**: Pretrained classifier model for 3 different classes based on Siamese NN backbone.
**annotation_utils**:Notebook includes codes on preprocessing data for object detector and classifier.
**Initial_SNN_Model_Training_Phase_1/2**: Consists of details on extraction of picture data required for training along with progress and changes made on the model so far.
