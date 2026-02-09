# Beyerdynamic DT 880 Pro EQ Profiles for EasyEffects

This repository provides high-precision Equalizer presets for the **Beyerdynamic DT 880 Pro (250 Ohm)** headphones, specifically optimized for **EasyEffects** (PipeWire) on Linux. These profiles are meticulously based on the **Harman AE/OE 2018 Target** measurements provided by **Oratory1990**.

## 🎧 Overview

The DT 880 Pro is an industry-standard analytical headphone, but it features the characteristic "Beyer Peak" in the treble and rolled-off sub-bass. These presets correct the frequency response to achieve professional-grade tonal balance.

### Profiles Included

1. **Fresh Pads (`dt880-pro-new-pads.json`)**: Optimized for new or stiff ear pads.
   * **Preference Rating**: Increases from **88/100** to **100/100**.
   * **Preamp Gain**: -5.4 dB.
2. **Worn Pads (`dt880-pro-old-pads.json`)**: Tuned for softened or compressed older ear pads.
   * **Preference Rating**: Increases from **83/100** to **107/100**.
   * **Preamp Gain**: -11.0 dB (Required for high-gain bass compensation).

---

## 🎨 Personal Preference & Fine-Tuning

The following bands are intended to be adjusted according to your personal taste without ruining the overall tonal balance:

### For Fresh Pads Profile

* **Bass (Band 1 - 105 Hz Lo-shelf)**: Adjust gain to preference.
* **Warmth (Band 2 - 200 Hz Bell)**: Adjust gain to preference.
* **Airiness (Band 10 - 10000 Hz Hi-shelf)**: Adjust gain to preference.

### For Worn Pads Profile

* **Bass (Band 1 - 100 Hz Lo-shelf)**: Set to +8.5 dB by default to compensate for pad wear.
* **Warmth (Band 2 - 210 Hz Bell)**: Adjust to control vocal thickness.

---

## 🛠 Technical Recommendations

* **Prevent Clipping**: Both profiles use negative **Preamp Gain** to provide necessary headroom for bass boosts. Use a physical volume knob (e.g., on a **MOTU M4**) to compensate for volume loss instead of increasing digital gain.
* **Buffer & Latency**: If you experience audio crackling (Xruns), check your status with `pw-top`. Increasing your PipeWire Quantum to **1024** or **2048** is recommended for stability.
* **Filter Accuracy**: Profiles are configured in **IIR Mode** using **RLC (BT)** logic for maximum mathematical fidelity to the original measurements.

---

## 📜 Credits

* Measurements and frequency analysis by **Oratory1990** ([full list](https://www.reddit.com/r/oratory1990/wiki/index/list_of_presets/)).
* EQ profile formatting and EasyEffects optimization by this repository's contributors.

---

## ⚖️ License

This project is licensed under [CC BY-NC 4.0](http://creativecommons.org/licenses/by-nc/4.0/).
**Free for personal use, but commercial use is strictly prohibited.**
