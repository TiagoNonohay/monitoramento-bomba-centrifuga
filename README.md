# Centrifugal Pump Monitoring — First Look at Telemetry Data

Hey! This project is a quick study on industrial signals and predictive maintenance basics for rotating equipment (specifically a centrifugal pump). The goal here was just to take some raw sensor data and see what we can learn about the machine's mechanical condition.

## What's Being Tracked
- **`temperatura_c`**: Operating temperature (°C)
- **`vibracao_mms_rms`**: Vibration velocity (mm/s RMS)
- **`pressao_bar`**: Discharge pressure (bar)
- **`estado`**: Pump status (`RUNNING` or `STOPPED`)

<img width="986" height="788" alt="image" src="https://github.com/user-attachments/assets/d2e59098-1b1a-405d-a2b0-7b69cbf852c8" />

## Initial Thoughts & Insights
- Some quick bumps in vibration and temp while `RUNNING` probably mean small process load changes or transient noise.
- The sudden drop in pressure and vibration around 10:55 clearly marks when the pump turned off (`STOPPED`).

## Data Limitations (Keeping it Real)
- **Synthetic Data:** Built this dataset purely to practice time series analysis.
- **Missing Tech Specs:** No pump nameplate details, RPM, bearing types, or performance curves (H-Q) included.
- **Not a Full Diagnosis:** We can't confirm or rule out actual mechanical faults like cavitation, misalignment, or unbalance with just this setup.
