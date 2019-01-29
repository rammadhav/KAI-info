# Kai
* Kai is the wearable band which allows to perform the  actions and inetract with the Device through gestures.
* The interactions between the KAI and the device are done by using the Bluetooth 5.0 technology.
* It allows to communicate with the device & programs.
* All the kai gestures that are performed usng KAI are sent to the dongle.
* The dongle is connected to the USB port.
* We can connect the multiple KAI's to one dongle.
* From the Dongle the gestures data is sent to the SDK.
# Architecture of KAI
* The KAI architrcture consists of  components<br>
1)SDK<br>
2)Control center Module<br>
3)KAI control center<br>
4)JSON<br>
5)CSharp<br>
6)Python<br>
# SDK
* SDK acts as the interface between hardware and software.
* SDK Reads the guestures data from the dongle and decode the codes and sends to the control center module.
* It is the middleware in the Architecture of KAI.
* It also has two types of communication 
 1)Web Socket Server
 2)Process 
# Control  Center Module
* The control center module consits of different modules the decoded data is sent to the respective module to perform the task.
* It also have the different data types to identify the gesture data.
### Types of Datatypes:
* **Gyroscope**<br>
* **Accelerometer**<br>
* **Magnetometer**<br>
* **Pyr data**

# KAI control center
* KAI control center is the User side application.
* It has the information of the battery or the battery indicater.
* User can set the different gesture actions to be porformed in an Application.
* The different gesture actions are **Pitch**,**York**,**Role**.
* Control center and the KAI control center does not posses any connection between each other but runs parallelly the same task or the instruction.
# JSON Format :
* JSON is used for the **Authentication of the user**,**Setting the Capabilities**,**Getting Capabilities**,**Fingure calibration**,**IMU Calibration**,**List Connected KAI's**.
### Authentication of the user:
* The User need to login at SDK by providing the ModuleID and ModuleSecret.
### Setting the Capabilities:
* Setting the several data types and declaring the gestures either it is true or false.
### Finger Calibration:
* Finger Calibration is done for the accuracy check of the fingures and  its position.<br>
### IMU Calibration:
* IMU Calibration is done for the accuracy check of  the gestures and the hand position.
* The calibrations are need to be by placing the device in the zero position.
### List Connected KAI's:
* The list of the connected KAI's are displayed. 
