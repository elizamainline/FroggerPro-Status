# FroggerPro Mainline Linux Status

Mainline Linux hardware support status for the **Nothing Phone (4a) Pro** (`froggerpro`).

This repository tracks the current state of the mainline Linux bring-up.

> [!NOTE]
> The status describes hardware support on mainline Linux, not Android / Nothing OS compatibility.

## Status

| Component | Status | Notes |
|---|---|---|
| Boot | ✅ Works |
| UFS | ✅ Works | Internal storage works |
| USB peripheral | ✅ Works | USB gadget/peripheral mode works |
| USB host / OTG | ✅ Works | USB host mode works |
| Display | ✅ Works | Display output works |
| GPU | ✅ Works | Adreno GPU acceleration works with Mesa |
| High refresh rate | ✅ Works | 120 Hz tested |
| Touchscreen | ✅ Works | Touch input works |
| Hardware buttons | ✅ Works | Power / volume buttons work |
| Wi-Fi | ✅ Works | Wi-Fi works |
| Bluetooth | ✅ Works | Bluetooth works |
| Audio playback | ✅ Works | Speakers / audio output works |
| Microphones | ✅ Works | Microphone input works |
| Battery fuel gauge | ✅ Works | Battery percentage and status are available |
| Haptics | ✅ Works | Haptic feedback works |
| Camera flash | ✅ Works | LED camera flash works |
| Proximity sensor | ✅ Works | Proximity sensing works |
| Ambient light sensor | ✅ Works | Ambient light sensing works |
| Accelerometer | ✅ Works | Accelerometer works |
| Gyroscope | ✅ Works | Gyroscope works |
| Magnetometer | ✅ Works | Magnetometer works |
| SIM detection | ✅ Works | SIM cards are detected |
| Mobile data | ✅ Works | Cellular data works |
| 5G | ✅ Works | Working 5G connection achieved |
| Charging | ⚠️ Partial | Charging works, but support is not yet considered complete |
| Modem | ⚠️ Partial | Cellular functionality works, including 5G, but the modem stack still needs more testing |
| NFC | ⚠️ Partial | Controller communicates, but NCI/polling still has issues |
| Sensors / DSP stack | ⚠️ Partial | Individual sensors work, but the overall sensor/DSP stack may still need additional integration and testing |
| Main camera | ❌ Broken | Camera pipeline does not currently produce a usable image |
| Ultrawide camera | ❌ Broken | Not working |
| Front camera | ❌ Broken | Not working |
| Camera autofocus | ❌ Broken | Camera subsystem is not yet usable |
| Fingerprint reader | ❌ Broken | Not working |
| Automatic brightness | ❌ Broken | Automatic brightness control is not working |
| GPS / GNSS | ❔ Untested | |
| Suspend / resume | ❔ Untested | |
| Deep sleep | ❔ Untested | |
| Thermal management | ❔ Untested | |

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

Some subsystems, especially the modem, cameras and power management, may still require additional debugging even where basic functionality is already available.
