cd "%userprofile%\Downloads"
adb root
adb remount
adb push weatherv2.apk /system/app/
adb push weatherv3.apk /system/app/
adb shell chmod 644 /system/app/weatherv2
adb shell chmod 644 /system/app/weatherv3
adb reboot
