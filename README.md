# Multi-scenario Heterogeneous UAV Energy Consumption Dataset (MH-UECD)
To evaluate the performance of energy consumption models across diverse flight scenarios and heterogeneous UAV types, we construct the Multi-scenario Heterogeneous UAV Energy Consumption Dataset (MH-UECD).

## 💾 Dataset Download
You can download the processed dataset (`.zip`) directly from the link below:
👉 **[Download Link: Release v1.0](https://github.com/Liangqi716/MH-UECD/releases/tag/v1.0)**

## 📂 Dataset Structure

The dataset is organized hierarchically by **UAV type** and **environmental conditions**, containing approximately **1,760** flight trajectories in total.
```text
dataset/
├── {uav_type}/                 # 5 Categories: Fixed-wing, VTOL, Rotary-wing (x3)
│   ├── wind_{speed}_{dir}/     # 20 Environmental conditions (Speed: 2-10m/s, Dir: 4 angles)
│   │   ├── {id}/               # Scenario ID (Varying cruise speed & payload)
│   │   │   └── processed.csv   # Time-series flight & energy data
│   │   └── ...
│   └── ...
└── ...
```
Note: The rotary_wing_2 directory contains fewer samples because its compact size limits the viable payload range.
