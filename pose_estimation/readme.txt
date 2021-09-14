**Human pose estimation**
Main aim of the project is to estimate human keypoints and draw the skeleton for input images and videos
Pose estimation involves 
1.Detecting bounding boxes from input image
    Each bounding box represents an induvidual person 
2.Normalising the image
    image is then resized into standard shape of (256,192)  
3.Predicting heatmaps for the image
    17 heatmap images are formed representing probability density of a certain keypoint  
4.Convert heatmap to coordinates
    search for the highest value in the heatmap and map it to the coordinates on the original image.
5.Drawing the skeleton
    Skeleton is drawn using the keypoints

alpha.ipynb
I have predicted poses for sample images(from frames folder) which is obtained from dividing video into 
frames and stored the skeleton images in (pred_frames) folder

video_model.ipynb
I have also done pose estimation for video(trial1.mp4) and drawn the pose and saved the video as trial2_output.mp4
