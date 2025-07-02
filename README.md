# spong-flutter
### spong flutter for mobile


Follow the official documentation of [Flutter](https://docs.flutter.dev/get-started/install/windows/mobile) 

**NOTE:** U don't need to setup android studio if u not running the apps in there, u only need the android SDK 35 and good to go.


#### Common Commands

##### Flutter

- flutter clean          : Clean build files
- flutter pub get        : Fetch dependencies
- flutter doctor         : Diagnose setup issues
- flutter devices        : List connected devices
- flutter build apk      : Build release APK
- flutter run            : run the project 
- flutter --version      : version check

##### ADB
- adb devices                     : list connected devices 
- adb connect (ip):(port)         : connect devices   
- adb pair (ip):(port)            : pair devices over wifi
- adb disconnect                  : disconnect all devices
- adb tcpip 5555                  : make static port
- adb kill-server                 : stop the adb server
- adb start-server                : start the adb server
- adb logcat                      : print log 


## 🧩 Development Environment

| Tool               | Version     |
|--------------------|-------------|
| Flutter            | 3.32.4      |
| Dart               | 3.8.1       |
| Android SDK        | 35          |
| Android Build Tools| 35.0.0      |
| Java (JDK)         | 17.0.9 (LTS)|
| Gradle             | 8.3         |

**NOTE:** For gradle ver i still don't know the compatibilty across flutter, dart, java, but personally i use 8.3


#### How to run the apps on real devices(Android)

There is some way to run it on your phone
1. Using your hotspot phone
2. Connect it with USB cable(USB debug)
3. Connect it wireless using the same wifi router

I recommend to use wireless method **(method 3)** since that is the most convenient way

**NOTE:** All of this way is need to use ADB (Android Debug Bridge), adb comes in with the android SDK **(assuming you're already download Android SDK 35)**


#### How to connect it wireless

1. **Go to Developer Options**

    - Open your phone's Settings

    - Scroll to "About phone"

    - Tap "Build number" 7 times until it says “You are now a developer”

    - Go back to Settings > System > Developer Options (or just search for “Developer options”)

2. **Enable USB Debugging**

    - In Developer Options, find and enable USB debugging
    
    - connect your phone to your pc via USB cable

    - run 'adb devices' to verify your devices is detected

    - run 'adb tcpip 5555' to make ip static

    - wait for a while and disconnect your phone

3. **Enable Wireless Debugging**

    - In Developer Options, find and enable Wireless debugging

4. **Tap on "Wireless debugging"**

    - This opens the wireless debugging options

    - You can see your phone IP & Port there, but since we already make static Port which is easier to connect, we can ignore the phone Port

    - On your run 'adb connect (ip):(port)'