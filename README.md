# csi_data

This project provides a time-series dataset with five categories, based on Received Signal Strength (RSS) readings.  
The five RSS data types correspond to different detection objects:

1. **One pedestrian**
2. **Two pedestrians**
3. **One bicycle**
4. **Two bicycles**
5. **One vehicle**

---

## Data Acquisition Hardware

The data collection device consists of:

- **ESP32** – a WiFi chip operating at **2.4 GHz**
- **SX127x** (where *x* represents 6 or 8) – used to generate and receive wireless signals at:
  - **915 MHz**
  - **433 MHz**

---

## Folder Structure: `dataset with different frequency and antenna height`

In this folder, each CSV file is named with information about the **frequency** and **antenna height**.

- The number **before** the underscore indicates the **antenna height** (in meters).
- The number **after** the underscore indicates the **frequency** (in MHz).

**Example:**  
`2_915.csv` → antenna height = 2 m, frequency = 915 MHz

---

## CSV File Format

- Each row of data begins with a **class label** (a number from 1 to 5) that distinguishes the detection object:

| Label | Object |
|-------|--------|
| 1     | One pedestrian |
| 2     | Two pedestrians |
| 3     | One bicycle |
| 4     | Two bicycles |
| 5     | One vehicle |

The remaining columns contain the RSS readings captured over time.

---

## Usage Notes

- The dataset is designed for time-series classification tasks.
- All measurements are raw RSS values; no preprocessing has been applied.
- Please cite this repository if you use the data in your research.

---

## Contact

For questions or collaborations, please open an issue or contact the project maintainer.
