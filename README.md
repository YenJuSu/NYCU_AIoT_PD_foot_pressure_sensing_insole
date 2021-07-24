# AIoT PD Foot Pressure Sensing Insole
This application is designed to show how to diagnose whether the users have the tendancy of Parkinson's disease using embARC. **AIoT PD Foot Pressure Sensing Insole** can measure user's gait, and then judge if the user is in high risk of the disease by NN Model. Every components of the device are detachable which makes it superior in mobility and convenience. Also, it can be controlled by Android App. The connection between the device and the Smartphone is based on Wi-Fi.

* [Introduction](#introduction)
	* [System Architecture](#system-architecture)
	* [Android App](#android-app)
* [Hardware and Software Setup](#hardware-and-software-setup)
	* [Required Hardware](#required-hardware)
	* [Required Software](#required-software)
	* [Hardware Connection](#hardware-connection)
* [User Manual](#user-manual)
	* [Before Running This Application](#before-running-this-application)
	* [Run This Application](#run-this-application)

## Introduction

**AIoT PD Foot Pressure Sensing Insole**

AIoT PD Foot Pressure Sensing Insole is a smart device which can be used to monitor the high-risk populations of Parkinson's disease. By daily monitoring, users can get the warning before everything get worse and look for the treatment as soon as possible. For PD patients, our project can also be a severity reference.


### System Architecture

### Android App
Our device can be controlled by AIoT-PD Android App. You can start/stop the measurement, see your foot pressure destribution and the final result on the App.

![app pic][0]
## Hardware and Software Setup
### Required Hardware
- 1 [Himax WE-I Plus EVB Endpoint AI Development Board][2]
<img src="hardware/Himax WE-I.jpg" alt="Himax" width="50%"/>

- 2 Raspberry Pi 3 B
- 2 [8-Channel 12-Bit ADC for Raspberry Pi (STM32F030)][3]
- 2 [RPi UPSPack V3][4]
- 2 4000mAh Lithium Battery
- 2 Pressure Sensing Insoles (Homemade)

- **The Pressure Sensing Insole shown below.**

	<img src="hardware/insole.jpg" alt="structure_diagram" width="30%"/>

	- 2 Insoles
	- 16 [FlexiForce A301 Pressure Sensor (111N)][1]

- **The physical picture shown below.**
<img src="hardware/photo.png" alt="photo" width="50%"/>

- **The structure diagram shown below.**
<img src="hardware/structure_diagram.png" alt="structure_diagram" width="70%"/>

### Required Software
- Metaware or ARC GNU Toolset
- embARC Machine Learning Inference Library
- AIoT-PD Android App

### Hardware Connection
- Connect **Himax WE-I Plus** to **Raspberry Pi** with USB cable(using UART)
- Connect **Raspberry Pi** to **8-Channel 12-Bit ADC** and **RPi UPSPack V3**(with Lithium Battery)
- Connect **pressure sensing insole** to **8-Channel 12-Bit ADC**
- Connect **Raspberry Pi** and mobile phone via WiFi

## User Manual
### Before Running This Application
- Download source code and AIoT-PD App from github
### Run This Application


[0]: doc/screenshots/APP.png	"app_pic" 
[1]: http://www.memstec.com.tw/productDetail.php?PNo=107	"FlexiForce A301 Pressure Sensor (111N)"
[2]: https://www.sparkfun.com/products/17256	"Himax WE-I Plus EVB Endpoint AI Development Board"
[3]: https://wiki.seeedstudio.com/8-Channel_12-Bit_ADC_for_Raspberry_Pi-STM32F030/	"8-Channel 12-Bit ADC for Raspberry Pi (STM32F030)"
[4]: https://www.raspberrypi.com.tw/10684/55/	"RPi UPSPack V3"
