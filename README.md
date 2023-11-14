## GVI_SYSU_Outdoor_Indoor_Dataset
This dataset contains complex indoor-outdoor converted GNSS-visual-inertial datasets collected in underground garages and buildings.


![data](https://github.com/SYSU-CPNTLab/GVI_SYSU_Outdoor_Indoor_Dataset/assets/74598384/2acb0519-cf70-4bb9-a803-9a535cc37263)


As depicted in Fig. \ref{equip}, our multi-sensor data acquisition device is versatile and can be utilized for both vehicle-mounted and handheld applications. The device integrates a variety of sensors, including a stereo camera and IMU from Realsense D455, two U-blox ZED-F9P modules from VRTK2 for RTK positioning information, and a smartphone for pressure sensor (barometer) measurements. All sensor data are synchronized using timestamps. We have collected five datasets in a variety of complex indoor-outdoor scenarios, encompassing outdoor environments, underground locations, and building interiors. 


##  Dataset Details
### The dataset is released in the form of rosbag and currently there are 10 rosbags available:

| name | duration | size |
| :--: | :------: | :--: |
| GVI_SYSU_UG1.bag | 413s | 9.47GB |
| GVI_SYSU_UG2.bag | 407s | 9.32GB |
| GVI_SYSU_CPNT.bag | 830s | 19.00GB |
| GVI_SYSU_Building_LC.bag | 606s | 13.87GB |
| GVI_SYSU_Building_L.bag | 511s | 11.71GB |
| GVI_SYSU_Building_C.bag | 591s | 13.54GB |



### The data items within the rosbag are listed below:
| topic | type | frequency | description |
| :---: | :--: | :-------: | :---------: |
| /camera/imu | sensor_msgs/Imu | 200Hz | IMU measurments from D455|
| /camera/infra1/image_rect_raw | sensor_msgs/Image | 30Hz | left camera |
| /camera/infra2/image_rect_raw | sensor_msgs/Image | 30Hz | right camera |
| /fixposition/corrimu | sensor_msgs/Imu | 200Hz | IMU measurments from VRTK2| 
| /fixposition/gnss1 | sensor_msgs/NavSatFix | 5Hz | GNSS1 RTK position from VRTK2| 
| /fixposition/gnss2| sensor_msgs/NavSatFix | 5Hz | GNSS2 RTK position from VRTK2| 


##  Dwonload
Data set download link：https://pan.baidu.com/s/16r17_SFyLk3FEW6osD0UhA 
Password：cpnt 

