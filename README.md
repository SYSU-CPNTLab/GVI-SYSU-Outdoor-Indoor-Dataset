## GVI_SYSU_Outdoor_Indoor_Dataset
This dataset contains complex indoor-outdoor converted GNSS-visual-inertial datasets collected in underground garages and buildings.


![data](https://github.com/SYSU-CPNTLab/GVI_SYSU_Outdoor_Indoor_Dataset/assets/74598384/2acb0519-cf70-4bb9-a803-9a535cc37263)


As depicted in Fig. \ref{equip}, our multi-sensor data acquisition device is versatile and can be utilized for both vehicle-mounted and handheld applications. The device integrates a variety of sensors, including a stereo camera and IMU from Realsense D455, two U-blox ZED-F9P modules from VRTK2 for RTK positioning information, and a smartphone for pressure sensor (barometer) measurements. All sensor data are synchronized using timestamps. We have collected five datasets in a variety of complex indoor-outdoor scenarios, encompassing outdoor environments, underground locations, and building interiors. 


##  Dataset Details
### The dataset is released in the form of rosbag and currently there are 10 rosbags available:

| name | duration | size |
| :--: | :------: | :--: |
| GVI_SYSU_UG1.bag | 14'39" | 9.47GB |
| GVI_SYSU_UG2.bag | 7'29" | 9.32GB |
| GVI_SYSU_CPNT.bag | 5'16" | 19.00GB |
| GVI_SYSU_Building_LC.bag | 11'09" | 13.87GB |
| GVI_SYSU_Building_L.bag | 3'19" | 11.71GB |
| GVI_SYSU_Building_C.bag | 2'49" | 13.54GB |



### The data items within the rosbag are listed below:
| topic | type | frequency | description |
| :---: | :--: | :-------: | :---------: |
| /camera/image_raw | sensor_msgs/Image | 20Hz | monocular camera |
| /camera/ueye_info | ueye_cam/UEyeInfo | 20Hz | camera info |
| /rtimulib_node/imu | sensor_msgs/Imu | 200Hz | IMU |
| /lbl_1 | lbl_data/LBLdata | 1Hz | #1 acoustic bouy measurements of LBL| 
| /lbl_2 | lbl_data/LBLdata | 1Hz | #2 acoustic bouy measurements of LBL| 
| /lbl_3 | lbl_data/LBLdata | 1Hz | #3 acoustic bouy measurements of LBL| 
| /lbl_4 | lbl_data/LBLdata | 1Hz | #4 acoustic bouy measurements of LBL| 
| /fix | sensor_msgs/NavSatFix | 1Hz | Trajectory with noise. |
| /barometer_node/depth | sensor_msgs/FluidPressure | 60Hz |  PS height measurement|
| /barometer_node/pressure | sensor_msgs/FluidPressure | 60Hz | PS raw measurement | 
| /barometer_node/temperature | sensor_msgs/Temperature | 60Hz | Temperature |
| /rtimulib_node/mag | sensor_msgs/MagneticField | 200Hz | MagneticField measurement | 

##  Dwonload
Data set download link：https://pan.baidu.com/s/16r17_SFyLk3FEW6osD0UhA 
Password：cpnt 

