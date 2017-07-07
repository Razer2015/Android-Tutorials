---
layout: default
---

# [](#header-1)APK Library Adding

In this tutorial, I will show you how to add _armeabi-v7a_ libraries to an _arm64-v8a_ APK to make it work on both devices.


### Prerequisites

1.  [7-Zip Installed](http://www.7-zip.org/download.html)
1.  [Signing Tools](https://goo.gl/cgchTP).
1.  APK where to add the libraries (amr64-v8a one)
1.  APK where from you get the required libraries (armeabi-v7a one)

![How the folder looks like before starting](https://i.gyazo.com/868330bafb42928f581890413a04303a.png)


### 1. Extract the needed libraries
#### 1.1 Open the armeabi-v7a APK
Right click -> 7-Zip -> Open
![Open with 7-Zip](https://i.gyazo.com/4fb9675f0af517063ce6061d52e8d01d.png)
#### 1.2 Go to the lib -folder
![Change to lib folder](https://i.gyazo.com/1d47f70a28e28a557087d80480a02365.png)
#### 1.3 Extract the folder
Drag the armeabi-v7a out
![Extract the armeabi folder](https://i.gyazo.com/332e937d7690f84441d746d7328cfaf6.png)

### 2. Add them to the another APK
#### 2.1 Add the folder
Open _**arm64-v8a**_ APK with _**Z-7ip**_ and drag the _**armeabi-v7a**_ folder in the _**lib**_ -folder

Answer **yes** to the confirm prompt
![Add the libraries](https://i.gyazo.com/6e99de2dca735c41357b2a6ac16d7674.png)
#### 2.2 How it will look like when done
![Final look](https://i.gyazo.com/eae39c786875f2707075da5368952ad4.png)

### 3. Sign the APK
Now we need to re-sign the APK because we modified it. It won't install unless we do this.

#### 3.1 Signing
Double click the sign_improved.bat and select the correct APK number.

Wait for it to finish and you are **DONE**!
![Signing the APK](https://i.gyazo.com/c0328fac9efc3a38b0b29e7be6b4ab22.png)
