Our assignment is Project A. The dataset is taken from http://www.nlpr.ia.ac.cn/pal/trafficdata/recognition.html and has total of 4170 traffic sign images.

From our coding, we succeed to detect and segment out the traffic sign images based on 3 main shape: rectangular, circular and triangular traffic sign shape.

The performance of our algorithm reaches our expectation with accuracy about 81.39%.

The accuracy is calculated based on IOU measure. The IOU value is intepreted as following:
       A IOU value >= 0.5 means correct segmentation of traffic sign
       A IOU value ranges between 0 and 0.5 means bad segementation of traffic sign
       A IOU value = 0 means not accurate segementation because the predicted area does not intersect with the actual area of the traffic sign at all
       
From our algorithm, we record and count the total correct segmented images (IOU >= 0.5), total bad segmented images (0 < IOU < 0.5) and total segmented images with IOU = 0
        total correct segmented images with IOU measure >= 0.5 is 3394
        total bad segmented images with value range between 0 < IOU < 0.5 is 626
        total of segmented images with IOU = 0 is 150

We display out the good segmented traffic sign images, bad segmented images and zero IOU images with both the IOU value, actual and predicted bouding box area on the images.
