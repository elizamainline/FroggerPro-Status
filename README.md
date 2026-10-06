# FroggerPro Mainline Linux Status

Mainline Linux hardware support status for the **Nothing Phone (4a) Pro** (`froggerpro`).

This repository tracks the current state of the mainline Linux bring-up.

This is an active bring-up project. A component marked **Works** means that its basic functionality has been successfully tested, but it does not necessarily mean that the implementation is production-ready or suitable for daily use.

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
| Camera actuators | ✅ Works | Lens actuators / autofocus control work |
| Camera flash | ✅ Works | LED camera flash works |
| Proximity sensor | ✅ Works | Proximity sensing works |
| Ambient light sensor | ✅ Works | Ambient light sensing works |
| Accelerometer | ✅ Works | Accelerometer works |
| Gyroscope | ✅ Works | Gyroscope works |
| Magnetometer | ✅ Works | Magnetometer works |
| NFC | ✅ Works | NFC works |
| GPS / GNSS | ✅ Works | GNSS positioning works |
| Glyph Matrix | ✅ Works | Glyph Matrix works |
| SIM detection | ✅ Works | SIM cards are detected |
| SMS | ✅ Works | SMS messaging works |
| Mobile data | ✅ Works | Cellular data works |
| 5G | ✅ Works | 5G connectivity has been successfully tested |
| Modem | ⚠️ Partial | SIM detection, SMS and mobile data, including 5G, work; overall modem stability and remaining telephony functionality still need more testing |
| Fingerprint reader | ❌ Broken | Not working |
| Calls | ❔ Untested | Voice calls have not been tested yet |
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

## Disclaimer

This project is experimental and is provided **as-is, without any warranty**.

Use it at your own risk. I am not responsible for data loss, hardware damage, broken devices, or any other issues resulting from using this work.

Hardware marked as **Works** indicates that it has worked in my testing; it does not guarantee that it will work reliably in every configuration or environment.
