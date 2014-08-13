#Android-App-Decompiling
=======================
##Tools for Android App Decompiling
1) Winrar/Winzip/7Zip (Recommended 7Zip since open source) download link http://www.7-zip.org/download.html
2) JDGui (or any java decompiler) download link http://code.google.com/p/innlab/downloads/detail?name=jd-gui-0.3.3.windows.zip
3) dex2jar download link http://code.google.com/p/dex2jar/downloads/detail?name=dex2jar-0.0.9.15.zip

Steps

1) Now just extract all the archives to anywhere and open the .apk file (android app) file with winrar/7Zip and extract is also.
2) Now copy the “Classes.dex”(which contains all the source code of the android App) file from android app folder into dex2jar extracted folder and run following command on command prompt(windows).
3) cd <path of dex2jar folder>
4) dex2jar classes.dex (important make sure that jdk is installed on your system and path is set into environment variables and if not try this Go to Properties of My Computer->Advanced->Environment Variable->New and then variable Name=”path” Variable value=”path of JDK bin folder” and save the settings).
5) Now above command will create one executable Jar file with extension .jar into dex2jar folder.
6) Now goto JDGui folder where you will get an executable file with cup icon.
7) open the jd-gui.exe file and goto File->Open File…. and open the .jar file from dex2jar folder done ! then you will see the complete source code of the android “.apk” file including all the classes and packages and resources and you will get manifest.xml and layout files in the extracted “.apk” folder including all icons,images and sound also.
8) Note : The Above procedure might not work for Layout XML files or some other XML files like menu,animation etc. so for tha you can download Apktool.bat from https://code.google.com/p/android-apktool/
9) And apktool.jar from https://code.google.com/p/android-apktool/downloads/detail?name=apktool1.4.1.tar.bz2&can=2&q=
10) Copy the extracted files into “C:\WINDOWS” folder
11) And for de-compiling you can use command apktool d Apkfile.apk Folder_for_decompiling this will take some time and extract all content of Apk file.

(Note For More information about Apktool check http://www.xda-developers.com/android/guide-to-decompiling-and-recompiling-with-apktool/)