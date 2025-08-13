# This is a fork of a [Simple Qt screen rotation manager](https://github.com/GuLinux/ScreenRotator) with modifications for PineTab2

Reads data from accelerometer sensors and rotates the display accordingly.

In *PineTab2* screen and touchscreen normal position is portrait,  while for touchpad it is landscape. So whatever sensor reads, the screen and touchpad are always
in different directions.



I modified the code so that the screen, touchscreen, and touchpad work properly.



Code improvement and testing are needed.

## Compilation requirements

 - cmake
 - gcc
 - Qt5 (with modules x11extras, sensors)
 - xrandr
 - XInput (Xi)
 
On ubuntu, run the following command to install dependencies:
```
sudo apt install -y git cmake build-essential qtbase5-dev libxrandr-dev libxi-dev libqt5x11extras5-dev libqt5sensors5-dev 
```

## Building
```
git clone https://github.com/GuLinux/ScreenRotator
mkdir ScreenRotator/build
cd ScreenRotator/build
cmake -DCMAKE_POLICY_VERSION_MINIMUM=3.5 ..
make all
sudo make install
```

## Links

Main icon: https://www.iconfinder.com/icons/326583/orientation_rotation_screen_icon#size=256

