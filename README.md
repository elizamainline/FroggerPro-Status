# FroggerPro Mainline Linux Status

Mainline Linux hardware support status for the **Nothing Phone (4a) Pro** (`froggerpro`).

This repository tracks the current state of the mainline Linux bring-up.

> [!NOTE]
> The status describes hardware support on mainline Linux, not Android / Nothing OS compatibility.

## Status

| Component | Status | Notes |
|---|---|---|
| Boot | ✅ Works | Boots mainline Linux |
| UFS | ✅ Works | Internal UFS storage works |
| USB peripheral | ✅ Works | USB gadget/peripheral mode works |
| USB host / OTG | ✅ Works | USB host mode works |
| Display | ✅ Works | Display output works |
| GPU | ✅ Works | Adreno 722 acceleration works with Mesa |
| High refresh rate | ✅ Works | 120 Hz tested |
| Touchscreen | ✅ Works | Touch input works |
| Hardware buttons | ✅ Works | Power and volume buttons work |
| Wi-Fi | ✅ Works | Wi-Fi works |
| Bluetooth | ✅ Works | Bluetooth works |
| Audio playback | ✅ Works | Speakers and audio output work |
| Microphones | ✅ Works | Microphone input works |
| Battery fuel gauge | ✅ Works | Battery percentage and status are available |
| Charging | ✅ Works | Battery charging works |
| Haptics | ✅ Works | Haptic feedback works |
| Main camera | ✅ Works | Camera capture works |
| Ultrawide camera | ✅ Works | Camera capture works |
| Telephoto camera | ✅ Works | Camera capture works |
| Front camera | ✅ Works | Camera capture works |
| Camera flash | ✅ Works | LED camera flash works |
| Proximity sensor | ✅ Works | Proximity sensing works |
| Ambient light sensor | ✅ Works | Ambient light sensing works |
| Accelerometer | ✅ Works | Accelerometer works |
| Gyroscope | ✅ Works | Gyroscope works |
| Magnetometer | ✅ Works | Magnetometer works |
| SIM detection | ✅ Works | SIM cards are detected |
| SMS | ✅ Works | SMS messaging works |
| Mobile data | ✅ Works | Cellular data works |
| 5G | ✅ Works | 5G connectivity has been successfully tested |
| Modem | ⚠️ Partial | SIM detection, SMS and mobile data, including 5G, work; overall modem stability and remaining telephony functionality still need more testing |
| NFC | ⚠️ Partial | Controller communicates, but NCI/polling still has issues |
| Camera actuators | ❌ Broken | Lens actuators / autofocus control are not working yet |
| Fingerprint reader | ❌ Broken | Not working |
| Automatic brightness | ❌ Broken | Automatic brightness control is not working |
| DisplayPort / USB-C video | ❌ Broken | Not expected to work; the device only exposes USB 2.0 |
| Calls | ❔ Untested | Voice calls have not been tested yet |
| GPS / GNSS | ❔ Untested | Not tested yet |
| Suspend / resume | ❔ Untested | Not tested yet |
| Deep sleep | ❔ Untested | Not tested yet |
| Thermal management | ❔ Untested | Not fully tested yet |

### Legend

| Status | Meaning |
|---|---|
| ✅ **Works** | Working normally |
| ⚠️ **Partial** | Working, but with missing functionality or known issues |
| ❌ **Broken** | Currently unusable or unsupported |
| ❔ **Untested** | Not tested yet or status is unknown |

## Device

| | |
|---|---|
| **Device** | Nothing Phone (4a) Pro |
| **Codename** | `froggerpro` |
| **SoC** | Qualcomm Snapdragon 7 Gen 4 (SM7750-AB) |
| **CPU** | 1× Cortex-A720 @ 2.8 GHz + 4× Cortex-A720 @ 2.4 GHz + 3× Cortex-A520 @ 1.8 GHz |
| **GPU** | Qualcomm Adreno 722 |
| **Display** | 1260 × 2800 AMOLED, up to 144 Hz |
| **Memory** | 8 / 12 GB LPDDR5X |
| **Storage** | UFS 3.1 |

## Notes

This is an active bring-up project. A component marked **Works** means that its basic functionality has been successfully tested, but it does not necessarily mean that the implementation is production-ready or suitable for daily use.

A large part of the hardware is already functional, including accelerated graphics, display, audio, microphones, Wi-Fi, Bluetooth, sensors, USB host mode, battery charging, cameras, SMS and cellular data.

The main areas still requiring work are the **modem stack, NFC and camera actuators**. All camera sensors can capture images, but lens actuator / autofocus control is not working yet.

DisplayPort / USB-C video output is not expected to become available because FroggerPro exposes only USB 2.0.

## Disclaimer

This project is experimental and is provided **as-is, without any warranty**.

Use it at your own risk. I am not responsible for data loss, hardware damage, broken devices, or any other issues resulting from using this work.

Hardware marked as **Works** indicates that it has worked in my testing; it does not guarantee that it will work reliably in every configuration or environment.
