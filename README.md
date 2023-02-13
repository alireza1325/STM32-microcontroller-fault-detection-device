# STM32-microcontroller-fault-detection-device
Development of a smart gadget for fault detection in rotating machines by implemention of Mahalanobis Distance (MD) on an MCU

Unlike uclidian distance, Mahalanobis Distance considers correlation in the data. So the MD was implemented on MCU to detect distance between an unseen data and machine's healty data. If the distance was greater than the threshould, the signal will be consider as unlhealty. 29 features were extracted from raw vibration data and the used to calculate the MD of data.

![image](https://user-images.githubusercontent.com/57262710/218378929-ba805cec-e9ac-4928-bd70-5a2df2b62eb2.png)

The algorithm flowchart is illustrated in figures below.

![image](https://user-images.githubusercontent.com/57262710/218379558-79772c4e-3c7b-416d-8c84-08c77c07e12c.png)
![image](https://user-images.githubusercontent.com/57262710/218379643-46b8da68-ee6c-42ac-82dd-a6a858db997d.png)

The whole processes of data acqusition, feature extraction and novelty detection were implemented on an MC the device shown in below figure was built. 

![image](https://user-images.githubusercontent.com/57262710/218379224-d93323f9-f806-4ac0-9550-5745fb95df5e.png)

A graphical user interface was also designed to show the progress of learning process and percentage of fault.
![image](https://user-images.githubusercontent.com/57262710/218379307-949d311d-96ea-4ec4-aaa4-446a5def12f5.png)


