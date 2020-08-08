# Face_Recognition_App

One of the most fun projects I had the pleasure to work on.
The app process an image that was uploaded by the user and predicts to who the image belongs to.
The steps to completion were:

## Structuring the data.

- Using the cv2 library the images were changed into greyscale.

- Images less than 60x60 were deleted.

- Images less than 100x100 were resized.

- The images are then cropped to have a fixed size.
 

## Data Preprocessing

- Images with missing features were removed

- The images were normalized (min and max scaling)

- Images are then transformed into Eigen Images

 
## Training the model

- Model is trained using sklearn and then evaluated

- Model is tuned

- ROC and AUC score successfully rate 0.89


## Pipeline models
 
- Step - 1: read image

- Step - 2: convert into gray scale

- Step - 3: crop the face (using haar cascade classifier)

- Step - 4: normalization (0-1)

- Step - 5: resize images (100,100)

- Step - 6: Flattening (1x10000)

- Step - 7: subtract with mean

- Step - 8: get eigen image

- Step - 9: pass to ml model (svm)
