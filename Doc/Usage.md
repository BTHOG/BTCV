![BT logo](http://brookmantech.com/img/logo.png "logo")
# BTCV

## Usage

### Description Screen

![01](img/01.jpg "01")

#### 1. Main View

#### 2. Context Menu

This is right-click context menus. You can show control panel(```Controller```).

#### 3. Status Bar

You can see frame rate. The right side shows ``` USB Communication Speed ```, the left side shows ``` Digital Image Process Speed ```.  
The frame rate depends on the specifications of your PC. This software does not guarantee 30 fps operation. Please refer to the frame rate value for operation.

#### 4. Controller

You can operate the camera with this panel.

##### Reset

Initialize the CIS/FPGA.

##### Setting Write

You can write CIS/FPGA settings from files.  
The files in the directory containing the exe file is displayed in the dropdown list, but you can also specify it directly.

##### Run / Stop

Run Preview / Stop Preview

##### Mode / SaveNum / SavePath / Capture

You can save images.

If you select ```BurstBMP``` or ```BurstRaw```, multiple images can be stored consecutively, but this software do not guarantee 	grabbing at max rate.  
If you want to acquire images at the maximum rate, please use ```RecRaw```.

##### iris

You can change the Exposure Time.

##### AGain

You can change Analog Gain (PGA).

##### bitshift / bitshift(sub)

This sensor has deeper bit depth. In order to display in Windows OS, it must be limited to 8 bits.  
When set to ``` 0 ```, the lowest 8 bits(LSB) are displayed.  
When set to ``` 4 ```, it displays 4 to 11 bits.

If you use ``` bitshift(sub) ```, you can make different settings with split screen.

Since WhiteClip processing is not implemented, it is necessary to pay attention to color misregistration at saturation.

##### Scale

You can change the image size.

##### Offset

You can change the black level.

##### DarkSub

You can use dark image subtraction for defect correction and black level correction.  
The files in the directory containing the exe file

This software refer ```dark.bin``` in the directory containing the exe file as a dark image.

##### SoftHob

Perform horizontal noise reduction process.

| item | Description |
| :--- | :--- |
| Off | |
| Left | use HOB on Left sides |
| Both | use HOB on both sides |
| Linear | Linear interpolation is performed on the left and right using HOB on both sides  |

##### Sort

If you want to see an image where pixels are aligned correctly, you need to set it exactly.

The default setting is ```StaggerL```.

##### Rgain / BGain

Set the color gain.

##### Demosaic

| item | Description |
| :--- | :--- |
| Through | Display image data as close to raw as possible. For analysis. |
| Off | Display image without demosaicing. |
| On_Mono | Display image with demosaicing and grayscale conversion. |
| On_Color | Display image with demosaicing. |
| Quadrant | For analysis. |
| QuadColor | For analysis. |
| Binning | Only for binning drive. |

This software does not process gamma or color matrix.  
If you want an image that is close to the actual development processing, you need to develop from raw data yourself.

Please be aware that this is an evaluation environment for sensors.
