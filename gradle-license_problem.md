After installing CodeWorksforAndroid the installed folder should looks like following (I installed here in D: drive).
![](https://github.com/goopymoon/goopymoon.github.io/blob/master/Image/codeworks_installed_root.PNG)

If android-sdk-windows has folder of same name (such as android-sdk-windows/android-sdk-windows) gradle suffers from android license problem. I don't know exactly when this happens in Windows OS but it happens.
If passed installation accept Edit/Project settings.../Platforms/Android/Acceopt SDK License then android-sdk-windows/licenses/android-sdk-license file will be generated. The license file contains following hash value.

![](https://github.com/goopymoon/goopymoon.github.io/blob/master/Image/codeworks_installed.PNG)
![](https://github.com/goopymoon/goopymoon.github.io/blob/master/Image/android_license.PNG)
