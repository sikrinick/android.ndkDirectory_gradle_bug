An example of `android.ndkDirectory` bug for Android Gradle Plugin 3.5.0.

Steps to reproduce:
1. Change `classpath 'com.android.tools.build:gradle:3.4.2'` to `classpath 'com.android.tools.build:gradle:3.5.0'`
in `build.gradle` of this project.

Expected:  
Gradle syncs successfully.

Actual:  
For 3.5.0 Gradle throws an exception 
`extensionSupplier.get()!!.compileSdkVersion must not be null`  
Where:   
Build file `'/Users/sikri/StudioProjects/androidndkdirectorybug/app/build.gradle'` line: 5