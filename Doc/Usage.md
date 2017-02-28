![BT logo](http://brookmantech.com/img/logo.png "logo")
# BTCV

## Usage

### Description Screen

![01](01.jpg "01")

#### 1. Main View

#### 2. Context Menu

This is right-click context menus. You can show control panel("Controller").

#### 3. Status Bar

You can see frames per second. The right side shows ``` USB Communication Speed ```, the left side shows ``` Digital Image Process Speed ```.

#### 4. Controller

You can operate the camera with this panel.

- Reset

Initialize the CIS/FPGA.

- Setting Write

You can write CIS/FPGA settings from files.  
The files in the directory containing the exe file is displayed in the dropdown list, but you can also specify it directly.

- Run / Stop

Run Preview / Stop Preview

- Mode
- SaveNum
- SavePath

- iris

You can change the Exposure Time.

- AGain

You can change Analog Gain(PGA).

- bitshift
- bitshift(sub)

This sensor has deeper bit depth. In order to display on Windows, it must be limited to 8 bits.  
When set to ``` 0 ```, the lowest 8 bits(LSB) are displayed.  
When set to ``` 4 ```, it displays 4 to 11 bits.

If you use ``` bitshift(sub) ```, you can make different settings with split screen.

- ```Scale```

You can change the image size.

- Offset

- DarkSub

- SoftHob

Perform horizontal noise reduction process.

| item | Description |
| :--- | :--- |
| Off | |
| Left | use HOB on Left sides |
| Both | use HOB on both sides |
| Linear | Linear interpolation is performed on the left and right using HOB on both sides  | 

- Sort

If you want to see an image where pixels are aligned correctly, you need to set it exactly.

- Rgain
- BGain

- Demosaic
