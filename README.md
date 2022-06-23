# carturn-detection
For autonomous vehicles especially in India now-a-days autonomous driving vehicles are preferred over the driver based driving cars due to the heavy traffic and the lack of systematicness while driving on the roads. The system stated here can identify the turn signals namely left turn and right turn. The motive behind this project was to increase the accuracy and robustness of the drivers assistance systems in autonomous vehicles.

The important aspects of the collision avoidance and the driver's assistance is detecting the car turn signals. Unfortunately the previously studied systems have lacked robustness due to huge variability in the shapes and size of the vehicles, variations in the day brightness due to variable environments, cluttered environment and drivers misbehavioural intentions. We have developed a system that will detect the turn signals of the front vehicles and give alert signals. The proposed system uses ORB and DAISY feature extractor to extract the features from the images. 

The feature vector generated from ORB and DAISY is furthermore optimized using K-Means clustering algorithm. This huge feature vector is converted into 16 clusters. This optimized feature vector is trained on 5 different classifiers namely SVM, Decision Tree, Logistic Regression, KNN, Random forest . The accuracy obtained from these classifiers is as follow 82.79%, 68.23%, 57.90%, 84.34%,  80.55% respectively 

[Link to dataset](https://drive.google.com/drive/folders/1O7llkK1FYOWfi0VUd9Wmy0vkJHkHYC_b?usp=sharing)

| Dataset Class | No of Images |
|---------------|--------------|
| Left          | 7709         |
| Right         | 8141         |
| Negative      | 8676         |
| Total images  | 24526        |

# How to use?

- Step one: install all needed libraries via pip ( to-do: add requirements.txt)
- Step two: download the dataset and update the file path on your local machine or drive, if using collab.
- Step three: run each cell. I have documentated each cell block with a link to references/documentation.

The entire dataset prepartion and augmentation has been undertaken by me, feel free to use the dataset.
