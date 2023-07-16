# LibNDK Translation for arm64-v8a,armeabi-v7a,armeabi
### newbit @ xda-developers
Installs the Libhoodjni functions into your AVD.

### Description
Make support of arm apps on x86 and AVD for android 11

### Notes
* rc file is not needed anymore, mount binfmt_misc and register copies are now in service.sh
* system.prop is updated
* set_perm_recursive are updated
* /system/lib/liblog.so and /system/lib64/liblog.so are added
	* due to **cannot locate symbol "__android_log_set_logger"** Error, liblog.so is needed
	* [__android_log_set_logger](https://developer.android.com/ndk/reference/group/logging#group___logging_1ga0e29961fa7bd5904bfc142d795af1fd6) is available since API level 30.
	* ADB is fixed now now it support with adb
	* to test flash module and install your arm apps everything is working almost fine arm64v6a working

* ## Example 
* 
* ![DEMO](https://github.com/ALEX5402/libndk_translation_Module/blob/master/image.png)
