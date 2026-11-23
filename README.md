# StereoSplit 

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011-blue?style=for-the-badge&logo=windows" alt="Platform" />
  <img src="https://img.shields.io/badge/Release-v1.0.0-green?style=for-the-badge&logo=github" alt="Release" />
  <img src="https://img.shields.io/badge/License-MIT-orange?style=for-the-badge" alt="License" />
  <img src="https://img.shields.io/badge/Architecture-x64-purple?style=for-the-badge" alt="Architecture" />
</p>

<p align="center">
  <b>High-performance, low-latency audio routing & channel separation utility for Windows.</b><br>
  Route Left and Right stereo channels independently across different physical speakers, headphones, or virtual audio endpoints.
</p>

---

##  Key Features

-  **Independent Channel Routing**
  - Split standard stereo streams into separate Left and Right discrete output channels.
  - Route Left to one audio device (e.g. primary headphone) and Right to another (e.g. secondary speaker/earpiece).

-  **Multi-Device & Multi-Link Support**
  - Broadcast and synchronize audio across multiple connected audio interfaces simultaneously.
  - Mix and match USB DACs, Bluetooth devices, and 3.5mm analog outputs.

-  **Spatial Audio & 3D Separation**
  - Enhanced stereo imaging and spatial positioning for immersive listening, gaming, and production setups.
  - Directional sound separation designed for assistive listening and multi-speaker room layouts.

-  **Per-Channel Volume & Gain Controls**
  - Independent gain adjustment, mute toggles, and balance sliders for each destination.
  - Peak-level indicators to prevent clipping and audio distortion.

-  **Ultra-Low Latency Engine**
  - Built on high-performance Windows audio APIs with minimal buffer overhead.
  - Suitable for real-time applications, gaming, media editing, and live monitoring.

-  **Portable & Lightweight**
  - Zero complex installations or driver hacks — standalone `.exe` ready to run.
  - No background telemetry, minimal CPU and RAM footprint.

---

##  System Architecture

```
                       ┌───────────────────────┐
                       │   Windows Audio Host  │
                       └──────────┬────────────┘
                                  │ (Stereo Input)
                                  ▼
                       ┌───────────────────────┐
                       │      StereoSplit      │
                       │   Channel Processor   │
                       └──────────┬────────────┘
                                  │
                 ┌────────────────┴────────────────┐
                 ▼                                 ▼
      [ Left Channel Stream ]           [ Right Channel Stream ]
                 │                                 │
                 ▼                                 ▼
    ┌─────────────────────────┐       ┌─────────────────────────┐
    │     Audio Device A      │       │     Audio Device B      │
    │  (Headphones / Earbuds) │       │   (External Speaker)    │
    └─────────────────────────┘       └─────────────────────────┘
```

---

##  Quick Start

### 1. Download
Grab the latest pre-compiled binary from the **[Releases](https://github.com/iamdatdev/StereoSplit/releases/latest)** page:
-  **[Download StereoSplit.exe (v1.0.0)](https://github.com/iamdatdev/StereoSplit/releases/download/v1.0.0/StereoSplit.exe)**

### 2. Run
1. Double-click `StereoSplit.exe` to start the application (no setup wizard required).
2. Select your input stream or default system audio source.
3. Choose the target output devices for the **Left Channel** and **Right Channel**.
4. Adjust channel levels and hit **Start Routing**.

---

##  System Requirements

| Requirement | Specification |
| :--- | :--- |
| **Operating System** | Windows 10 (1903+) / Windows 11 (64-bit) |
| **Processor** | Dual-core 1.5 GHz or higher |
| **RAM** | 50 MB available RAM |
| **Audio Hardware** | Compatible Windows-recognized sound card / USB / Bluetooth device |

---

##  Typical Use Cases

- **Shared Audio on Two Headsets**: Listen with a friend using two pairs of earphones, routing each channel or dedicated streams to individual listeners.
- **Multi-Room & Spatial Testing**: Route left/right soundstage elements to physically separated speaker monitors for acoustics calibration.
- **Gaming & Directional Cues**: Isolate directional audio tracks to specialized tactile transducers or dedicated side monitors.
- **Accessibility & Hearing Assistance**: Compensate for uneven hearing thresholds by tailoring gain and balance specifically per ear/device.

---

##  License

This project is licensed under the [MIT License](LICENSE) - feel free to use, modify, and distribute.
