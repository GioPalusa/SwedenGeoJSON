# SwedenGeoJSON
GeoJSON datasets representing the Kingdom of Sweden, including national borders, counties (län), municipalities (kommuner), and other administrative regions. Useful for mapping, GIS analysis, and applications that require structured geographic boundaries of Sweden.

<img width="258" height="508" alt="Skärmavbild 2026-03-23 kl  22 08 08" src="https://github.com/user-attachments/assets/1abad02a-0eb8-400e-bc52-c7ab8b1156ff" />
<img width="258" height="508" alt="Skärmavbild 2026-03-23 kl  22 08 53" src="https://github.com/user-attachments/assets/f9ebb737-565b-4dd7-b097-21968d01bc24" />
<img width="258" height="508" alt="Skärmavbild 2026-03-23 kl  22 09 37" src="https://github.com/user-attachments/assets/b5dab538-3267-4409-aec2-5afe0b1b2227" />

# Sweden Administrative Boundaries (2026)

GeoJSON dataset containing Sweden's administrative boundaries for **2026** in WGS84 format.

The dataset represents the official administrative divisions of Sweden at the **start of the year 2026**.

Included administrative levels:

- **Rike** (Country)
- **Län** (Counties / Regions)
- **Kommuner** (Municipalities)

All geometries are provided as **GeoJSON** and use the coordinate system **WGS84 (EPSG:4326)**.

---

# Dataset Contents

The repository contains three datasets:

geojson/
rike.geojson
lan.geojson
kommun.geojson

Geometry type:
MultiPolygon

Each feature includes attributes describing the administrative unit, such as:

- `lanskod`
- `lansbokstav`
- `kommunkod`
- `beslutatnamn`
- `landskod`
- `referensdatumfran`
- `referensdatumtill`

---

# Dataset Description

The dataset **Kommun, län och rike** describes Sweden's administrative territorial divisions as polygon geometries.

Municipality boundaries are derived from property boundaries in the Swedish Real Property Register.  
County geometries are aggregated from municipalities, and the national boundary is aggregated from counties.

Because some administrative areas contain **exclaves**, geometries are represented as **MultiPolygon** objects.

This repository contains the **annual dataset for 2026**, representing the administrative divisions as they appear at the **beginning of the year (1 January 2026)**.

Annual datasets are commonly used for:

- statistical analysis
- historical comparisons
- geographic analysis
- mapping and visualization

---

# Source

The data originates from the official Swedish dataset:

**Kommun, län och rike**

Produced by:

- **Lantmäteriet** – current datasets and annual datasets from 2025 onwards
- **Statistics Sweden (SCB)** – historical annual datasets

Specification:

https://www.lantmateriet.se/globalassets/temawebbar/ngp/informationsspecifikation_kommun_lan_rike_test_1_rev32.pdf

---

# Data Processing

The original dataset is distributed by Lantmäteriet as **GeoPackage (.gpkg)** in the coordinate reference system **SWEREF99 TM**.

For this repository the data has been:

- converted to **GeoJSON**
- reprojected to **WGS84 (EPSG:4326)**

Source: Lantmäteriet – Kommun, län och rike

---
