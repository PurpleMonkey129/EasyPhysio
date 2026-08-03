# EasyPhysio DBT Analyzer 🫀

[![Version](https://img.shields.io/badge/version-2.1.1-blue.svg)](https://github.com/acadlabs/dbt-analyzer/releases/tag/v2.1.1)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20(64--bit)-lightgrey.svg)](https://acadlabs.in)
[![License](https://img.shields.io/badge/license-GPL--3.0-blue.svg)](LICENSE)

**EasyPhysio DBT Analyzer** is a high-performance desktop application for autonomic nervous system evaluation. It specializes in parsing BIOPAC (`.acq`) ECG recordings, automated/interactive R-peak detection, and performing Deep Breathing Test (DBT) Respiratory Sinus Arrhythmia (RSA) ratio calculations.

Developed by [acadLabs.in](https://acadlabs.in).

---

## 🌟 Key Features

- 📁 **BIOPAC `.acq` Signal Reader**: Direct parsing of BIOPAC `.acq` raw telemetry and ECG channel data.
- ⚡ **R-Peak Detection & Editing**:
  - Automated peak detection with dynamic thresholding slider.
  - Inverted lead support (Negative peak mode).
  - Manual peak insertion with apex auto-snapping and single-click peak deletion.
- 📈 **Interactive RR Tachogram**:
  - Time-series plot of RR intervals with synchronized zoom and scroll controls.
  - Color-coded RR interval classification (<600 ms, >1200 ms).
- 🫁 **Deep Breathing Test (DBT) & RSA Ratios**:
  - Automatic detection of expiratory (E) and inspiratory (I) RR interval extrema.
  - Live calculations for **Mean E:I Ratio**, **Median E:I Ratio**, and **Ratio of Means**.
  - **E:I Peak Edit Mode (New in v2.1.1)**: Interactive floating popup (`EIPeakPopup`) to manually override, designate, or clear expiratory/inspiratory peaks directly on the tachogram with real-time recalculations.
- 🚀 **Optimized & Self-Contained**:
  - Standalone application — **no Python or external dependencies required**.
  - High-performance UI built with PySide6 / Qt6.
- 💾 **Data Export**:
  - Export RR interval time-series to `.txt` or `.csv`.
  - Export structured DBT analysis summary reports suitable for Excel, SPSS, or R.

---

## 🚀 Download & Installation

Download the latest version from the **[Releases Page](https://github.com/acadlabs/dbt-analyzer/releases/tag/v2.1.1)**:

| Package | Description | Recommended For |
|---|---|---|
| 📦 **`EasyPhysio_DBT_Analyzer_v2.1.1_Setup.exe`** | Automatic Setup Installer | Most Windows Users |
| 📁 **`EasyPhysio DBT Analyzer v2.1.1.zip`** | Portable Edition | Users without Admin rights / USB drives |

### Installation Instructions

#### Option A: Windows Installer (`.exe`)
1. Download `EasyPhysio_DBT_Analyzer_v2.1.1_Setup.exe`.
2. Double-click to run the setup wizard and follow the on-screen instructions.
3. Launch **EasyPhysio DBT Analyzer** directly from your Desktop or Start Menu.

#### Option B: Portable Edition (`.zip`)
1. Download `EasyPhysio DBT Analyzer v2.1.1.zip`.
2. Extract the ZIP folder to a safe location (e.g., `C:\Program Files\EasyPhysio\` or `Documents`).
3. Open the extracted folder and double-click `DBT Analyzer - EasyPhysio.exe`.
> ⚠️ **Note:** Do not move `DBT Analyzer - EasyPhysio.exe` out of its folder. To create a Desktop icon, right-click the EXE → **Send to → Desktop (create shortcut)**.

---

## 📖 Quick Start Guide

1. **Load ECG Recording**: Click **Open** in the toolbar and select your `.acq` file.
2. **Adjust R-Peak Sensitivity**: Drag the threshold slider at the bottom to adjust detection sensitivity. Check **Negative** if R-peaks point downward.
3. **Manual Peak Corrections**:
   - **Add Peak**: Click directly on the ECG waveform (snaps to apex).
   - **Delete Peak**: Click an R-peak marker to highlight it red/green, then press `Delete`.
4. **Analyze DBT**: Click **Analyze DBT** in the toolbar to generate respiratory cycle metrics.
5. **E:I Peak Edit Mode**: Enable **E:I Edit Mode** on the tachogram to customize or clear inspiratory/expiratory peak markers with live metric recalculations.
6. **Export**: Click **Save DBT Results** to export tables to CSV or TXT.

---

## 🖥️ System Requirements

| Requirement | Specification |
|---|---|
| **Operating System** | Windows 10 / Windows 11 (64-bit) |
| **RAM** | 4 GB minimum (8 GB recommended) |
| **Storage** | 350 MB free space |
| **Display** | 1280 × 720 or higher |
| **Python** | **Not required** (Bundled executable) |

---

## 📄 License & Contact

Developed by **[acadLabs.in](https://acadlabs.in)**.  
Distributed under the GNU General Public License v3.0 (GPL-3.0). See `LICENSE` for details.

For custom software development, clinical integration, or support:  
📧 **contact@acadlabs.in**
