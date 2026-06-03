# AutoHotKey_Scripts
This program takes user input from an XInput controller and maps it to complex keyboard input. 
It is used to play games similar to Diablo 3 using a controller. 

A video explaining its uses and how to set it up can be found [here](https://youtu.be/xgfTRkbmkJE)

The main program was coded in the AutoHotKey scripting language. The windows form configuration application was coded using C#

## Windows 11 recompilation note

On Windows 11, the precompiled `Joystick to Keyboard Emulation.exe` from the release may fail with:

```text
Failed to initialize XInput: function not found
```

A working solution was to recompile the original, unmodified source locally instead of using the old precompiled EXE.

Tested working setup:

```text
Windows 11
AutoHotkey_H v1.1.33.10-H005 A32
Ahk2Exe for AutoHotkey v1.1.37.02a2
Base File: v1.1.33.10-H005 A32 AutoHotkeyA.exe
Source: ConfigurationForm/ConfigurationForm/AutoHotkey/Joystick to Keyboard Emulation.ahk
```

No source code changes were required. After local recompilation, an original Xbox One controller connected over Bluetooth worked correctly.

### Diablo III Defaults
![](https://github.com/bennybroseph/AutoHotKey_Scripts/blob/v2.1/ConfigurationForm/ConfigurationForm/Images/Controller%20Layout%20Diablo%20III.png)

### Path of Exile Defaults

![](https://github.com/bennybroseph/AutoHotKey_Scripts/blob/v2.1/ConfigurationForm/ConfigurationForm/Images/Controller%20Layout%20Path%20of%20Exile.png)


#### AutoLauncher for Diablo III
There is an **[AutoLauncher](https://github.com/VagnerDomingues/Diablo-III-PC-Joystick-AutoLauncher)** included to play Diablo III, It automatically starts the joystick-to-keyboard emulator when the game launches and closes it when the game exits, improving quality of life.