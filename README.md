# UBPG
General Information about the Upper Body Point Cloud Gestures Dataset (UBPG)

## Dataset Description
This a point cloud based gesture dataset captured by the Kinect camera using the Point Cloud Library. It contains 9 classes of gesture with 1 class for No Gesuture. The gestures are: 1. No Gesure, 2. Come, 3. Me, 4. No Thank You, 5. Money, 6. Peace, 7. Not Allowed, 8. OK, 9. I'm Sorry and 10. I Got It!. There were originally 5 subjects but 2 more subjects has been aadded (s6 and take-080218). Each subjects performed the gesture at least 30 times per gesture.

The subjects are organized according to the folder names and each file is named in the following format: 

cloud_[serial_number_in_folder]_label_[gesture_class_label]_reached_[duration_of_gesture_performance].ply

Note that most files do not have the `duration_of_gesture_performance` tag. This means that all preceeding frames before `duration_of_gesture_performance` tag are part of the same gesure performance. Be sure to maintain the original folders as files in different folders might have the same name.

To reference this dataset, use the paper below
```
Owoyemi, J., & Hashimoto, K. (2018). Spatiotemporal Learning of Dynamic Gestures from 3D Point Cloud Data. In 2018 IEEE International Conference on Robotics and Automation (ICRA) May 21-25, 2018, Brisbane, Australia (pp. 5929–5934). Brisbane. https://doi.org/10.1109/ICRA.2018.8460910
```


The dataset has also been used in the following paper:

```
Kingkan, C., Owoyemi, J., & Hashimoto, K. (2018). Point Attention Network for Gesture Recognition Using Point Cloud Data. In 29th British Machine Vision Conference (pp. 1–13). Newcastle. http://bmvc2018.org/contents/papers/0427.pdf
```

## Download link
You can download the datset from [here](https://1drv.ms/f/s!Ar0kGAMVBu3Ng6sJiqv2GIlOQhQYuw).

## Evaluation
We propose the following 3 tests for model evaluation.
Test 1: Train with 1/3 of the dataset and test with the remaining
Test 2: Train with 2/3 of the dataset and test with the remaining
Test 3: Train with half of the subjects and test with the remaining subjects
