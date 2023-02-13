# STM32-microcontroller-fault-detection-device
Development of a smart gadget for fault detection in rotating machines by the implementation of Mahalanobis Distance (MD) on an MCU.

The provided zip file is the source code of MCU to implement the algorithm as describe in the following sentences. It should be noted that STM32CubeIDE and STM32CubeMX were used to program the microcontroller.

Unlike euclidian distance, Mahalanobis Distance considers correlation in the data. So the MD was implemented in MCU to detect the distance between unseen data and the machine's healthy data. If the distance was greater than the threshold, the signal will be considered unhealthy. 29 features were extracted from raw vibration data and used to calculate the MD of data.

![image](https://user-images.githubusercontent.com/57262710/218378929-ba805cec-e9ac-4928-bd70-5a2df2b62eb2.png)

The algorithm flowchart is illustrated in the figures below.

![image](https://user-images.githubusercontent.com/57262710/218379558-79772c4e-3c7b-416d-8c84-08c77c07e12c.png)
![image](https://user-images.githubusercontent.com/57262710/218379643-46b8da68-ee6c-42ac-82dd-a6a858db997d.png)

The whole processes of data acquisition, feature extraction, and novelty detection were implemented on an MCU, and the device shown in the below figure was built. 

![image](https://user-images.githubusercontent.com/57262710/218379224-d93323f9-f806-4ac0-9550-5745fb95df5e.png)

A graphical user interface was also designed to show the progress of the learning process and the percentage of faults.
![image](https://user-images.githubusercontent.com/57262710/218379307-949d311d-96ea-4ec4-aaa4-446a5def12f5.png)

The device was tested on an experimental setup depicted in this figure:
![image](https://user-images.githubusercontent.com/57262710/218379890-0e66e311-dc68-42f3-ab09-006adddf5258.png)

And unhealthy state was created by adding some tiny masses on the motor to simulate an imbalanced fault. As shown in the figure below, the algorithm could detect most unhealthy machines' behavior. 
![image](https://user-images.githubusercontent.com/57262710/218380159-4b1a072a-f6b9-4c58-b7df-24c18765a0d4.png)


