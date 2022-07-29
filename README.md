# Aruco tags in Gazebo simulation

## Launching the bot 

Run the following command
```
roslaunch mybot mybot.launch
```
## Generating aruco tags in gazebo simulation 

1. Navigate to the Gazebo_models directory 
2. In the images folder add the .png images for the ar tags required. Note that they have to be resized to dimensions 170*170 px
3. Run the following command
```
./generate_markers_model.py -i <path to the image directory> -s <size of the model in mm> -w <white contour aroud the images; put 0 if not required>
```
5. The models should be present in ./gazebo/models (check hidden directories to get the gazebo directory)
6. In gazebo the models should be available in the model insert tab 
