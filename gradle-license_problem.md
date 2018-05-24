How to setup codeworks for android in Windows 10.

Run Setup.bat

Install Engine\Extra\AndroidWorks\Win64\CodeWorksforAndroid-1R6u1-windows.exe (I installed here in D: drive).
The installed folder should looks like the following. If android-sdk-windows has folder of same name (such as android-sdk-windows/android-sdk-windows) gradle suffers from android license problem. I don't know exactly when this happens in Windows OS but it happens.

![](https://github.com/goopymoon/goopymoon.github.io/blob/master/Image/codeworks_installed_root.PNG)

If you passed installation accept Edit/Project settings.../Platforms/Android/Acceopt SDK License then android-sdk-windows/licenses/android-sdk-license file will be generated. The license file contains following hash value.

![](https://github.com/goopymoon/goopymoon.github.io/blob/master/Image/codeworks_installed.PNG)
![](https://github.com/goopymoon/goopymoon.github.io/blob/master/Image/android_license.PNG)

Run Setup.bat again.
