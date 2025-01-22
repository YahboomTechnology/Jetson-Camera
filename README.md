# NVIDIA Jetson HD AI camera 8MP CSI interface IMX219 compatible with NANO/Xavier NX/TX2 NX/Orin
![](https://github.com/YahboomTechnology/Jetson-Camera/blob/master/Jetson_Camera.jpg)
# Introduction
This camera is suitable for Jetson Nano/Xavier NX/TX2 NX/Orin NX/Orin NANO. It adopts Sony IMX219 chip and CSI interface. The pixel is 800W, resolution is 1080P, and the field of view angle is 77°, 120° and 160°. It can be used to neural network, AI vision, real-time image recognition, AI smart robot cars and other fields. We will provide a transparent acrylic bracket for the camera, which can be mounted on the acrylic case.
# Features
* Camera for the Jetson Nano/Xavier NX/TX2 NX/Orin NANO/Orin NX board.
* Sony IMX219 chip, CSI interface.
* 8MP, 1080P resolution.
* 77° , 120°, 160° view angle.
* Wide range of applications.
* A reliable and beautiful acrylic bracket will be provided.
# How to enable CSI driver support in Jetpack
In order for the camera to be recognized by the Jetpack OS, you may have to enable the CSI driver support.
**Without CSI driver support enabled, the camera will not be recognized**.
1. Open up the terminal and run  
`sudo /opt/nvidia/jetson-io/jetson-io.py`
1. A menu will now appear.  Follow the options below to enable IMX219 support.  
`> Configure Jetson 24pin CSI Connector`  
`> Configure for compatible hardware`  
`> Camera IMX219 Dual`  
`> Save pin changes`  
`> Save and reboot to reconfigure pins`  
1. The OS is now configured with the CSI driver support enabled.  To test this run  
`sudo dmesg | grep imx219`  
and verify the output.  You will find the *bound* message for both ports if you have connected both cameras.  Something like the following:
```
[  604.226388] imx708 9-001a: tegracam sensor driver:imx708_v2.0.6
[  604.527906] tegra-camrtc-capture-vi tegra-capture-vi: subdev imx708 9-001a bound
[  604.529755] imx708 10-001a: tegracam sensor driver:imx708_v2.0.6
[  604.834263] tegra-camrtc-capture-vi tegra-capture-vi: subdev imx708 10-001a bound
```

# Required Best Buy Links
[Click here](https://category.yahboom.net/products/jetson-nano-camera)

# Please Contact Us
If you have any problem when using our robot after checking the tutorial, please contact us.

### WhatsApp:
+86 18682378128

### Technical support email: 
support@yahboom.com
