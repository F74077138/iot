# FoG Detection Sytem
A system to detect Freezing of Gait caused by Parkinson's disease.  
System consists of:  
1. Insole
2. Visualization application
3. Bluno controller application
4. Deep learning model

## Things to install
- Java
- Python 3.x
- Python packages (FastAPI, TensorFlow, etc.)
- IDE (VS Code, Android Studio, etc.)

## Installation

### Java
1. Go to Java official website [here](https://java.com/en/download/help/download_options.html).
2. Select which OS on which you are installing Java on.
3. Follow detailed guides.

### IDE: VS Code (Python)
1. Download VS Code [here](https://code.visualstudio.com/).
2. Once download is finished, start VS Code.
3. Go to Extensions tab on the left-hand side or click and hold (Ctrl+Shift+X).
    * If above instruction doesn't work, click View -> Command Palette.
    * Type "install", and select Extensions: Install Extensions.
4. Type "Python" in the extensions search field, select Python in the list, and click Install.
5. Install a Python interpreter [here](https://www.python.org/downloads/).
6. On menu bar, select Terminal -> New Terminal.
7. Verify installation using the command ```python3 --version```

### IDE: Android Studio (Java)
Refer the installation guide [here](https://developer.android.com/studio/install).

## App Deployment
Make sure device has version Android Oreo or higher.  
Below is the instruction on how to deploy app to device:
1. In Android Studio, make sure that in the Device Selection is the device you want to deploy in.
    * If No device is shown, it means target device is not found or device not properly plugged in.
    * Make sure your device has enabled developer option [here](https://www.digitaltrends.com/mobile/how-to-get-developer-options-on-android/).
2.  Once target device is found, click Shift + F10 or press the green arrow/Run Button  on the top right menu pane to deploy app to device.

Process might take a while before the app can run on the device.

## Server
Server is run locally on our laptop.
###### for Windows
Firewall must be deactivated to access server from mobile app.
###### for MacOs/Linux
No firewall deactivation needed.
##### Running the server
All dependecies / libraries must already be installed in order for it to run properly.  
Server file can be found in ```app.py```. Tor run the server, type:
```bash
uvicorn app:app --reload --host [IPv4 address]
```

## Things to change
1. ```Visualization.java```:
   * Line 60 & 61: Change insole mac address (Can be found by checking Bluetooth settings on any device).
   * Line 246 & 370: Change to current IPv4 address.
2. ```BLUNO (MainActivity.java)```:
   * Line 177: Change to current IPv4 address.

## Contributions
* Data Collection: 蔡孝龍 F74077120
* Model Development: 余更忠 F74077023
* App Development: 達愛娜 F74077138
* Server integration: 曾青山 F74075055
* Hardware: 常定利 F74067036
