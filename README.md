# Detection-of-Plant-Direction-in-an-Image

`Detection of plant direction in an image` is the project inspired from our college's Mega Expo Proble Statemet describes the autonomous survailance of crop using mobile Robot in agricultural farms.

### Approach for Classification: 
1. **Capturing an Image**
2. **Preprocessing the Image**
3. **Finetuning the pretrained `RESNET 50` model with our less training data**
    This whole Process is meant for only **Classification** of Image whether the image has a plant or not.

### Approach for plant Direction measurement : 
1. **Validating the RESNET 50 model with our validation set.**
2. **Testing is done by Giving an image to the model to predict whether image has plant or not.**
3. **If plant was detected, The image is splitted into patches and fed each patch to the model for prediction.**
4. **Checking Whether the plant is belongs to the left, right or center of an image.**

   This approach is inspired from the first object detection model called `OverFeat`.

**Tip :**
 We can also finetune the YOLO model parameters for precise plant location. Since it outputs both predicted class and the Bounding box coordinates.

 >> Due to time constraint we cannot annotate the plant images to fed to the YOLO model. So, we took help from `overfeat` since it is flexible and easy to access and code.
