# 🌍 Global EV Charging Stations & EV Models Dataset (2025 Snapshot)

**Author:** [Tarek Masryo](https://github.com/tarekmasryo) · [Kaggle](https://www.kaggle.com/datasets/tarekmasryo/global-ev-charging-stations)  
**Version:** v1.0 (2025-09-01)  
**License:** CC BY 4.0  


---

## 📌 TL;DR
A clean, analysis-ready dataset capturing the state of EV infrastructure in **2025**:  
- **242,418 rows** across **122 countries**  
- **11 tidy columns** describing charging sites  
- Companion files: country/world roll-ups + EV models  

---

## 🚗 Why this dataset?
Electric mobility is booming, but data is scattered, inconsistent, and full of gaps.  
This project offers a **single, clean CSV snapshot** plus contextual summaries, making it ideal for:  
- EV adoption analysis  
- Energy planning & sustainability research  
- Machine learning & dashboard prototyping  

---

## 📂 Files Included
- `charging_stations_2025_world.csv` — global stations (main file)  
- `country_summary_2025.csv` — per-country roll-up  
- `world_summary_2025.csv` — global KPIs  
- `ev_models_2025.csv` — companion EV model specs  
- `OCM_CC_BY_4.0.txt` — license text  
- `dataset-metadata.json` — structured metadata  

---

## 🗄️ Data Dictionary

### `charging_stations_2025_world.csv`
| Column          | Type   | Description                                  |
|-----------------|--------|----------------------------------------------|
| id              | int    | Unique station ID (OCM)                      |
| name            | str    | Station name                                 |
| city            | str    | City name                                    |
| country_code    | str    | ISO-2 country code                           |
| state_province  | str    | State/Province (if available)                |
| latitude        | float  | WGS84 latitude                               |
| longitude       | float  | WGS84 longitude                              |
| ports           | int    | Number of charging points at the site        |
| power_kw        | float  | Maximum charging power (kW)                  |
| power_class     | str    | Derived class (slow/fast/HPC)                |
| is_fast_dc      | bool   | True if `power_kw ≥ 50`                      |

### `country_summary_2025.csv`
| Column          | Type   | Description                         |
|-----------------|--------|-------------------------------------|
| country         | str    | Country name                        |
| total_stations  | int    | Number of stations                  |
| avg_ports       | float  | Avg. ports per site                 |
| avg_power_kw    | float  | Avg. power (kW)                     |
| ev_adoption_rate| float  | Estimated adoption rate (%)          |

### `ev_models_2025.csv`
| Column          | Type   | Description                         |
|-----------------|--------|-------------------------------------|
| model_id        | int    | EV model unique ID                  |
| brand           | str    | Manufacturer                        |
| model           | str    | Model name                          |
| battery_kwh     | float  | Battery capacity (kWh)              |
| max_range_km    | int    | Max driving range (km)              |
| fast_charging   | bool   | Supports fast charging (yes/no)     |

### `world_summary_2025.csv`
| Column          | Type   | Description                         |
|-----------------|--------|-------------------------------------|
| year            | int    | Year of snapshot                    |
| total_countries | int    | Countries included                  |
| total_stations  | int    | Global total stations               |
| total_ev_models | int    | Number of EV models tracked         |
| avg_global_power| float  | Global avg. power (kW)              |

---


---

## 💡 Suggested Uses
- Compare EV infrastructure across regions  
- Measure share of fast-DC vs slow charging  
- Build EV adoption dashboards  
- Train ML models for site clustering or adoption forecasting  
- Prototype routing/location tools for EV drivers  

---

## 📜 License & Attribution
- Charging station data: © Open Charge Map — CC BY 4.0  
  → “Contains data © Open Charge Map contributors.”  
- EV models: compiled from CC0-friendly sources. Attribution optional.  
 

---

## 🔑 Keywords
EV, Charging, Infrastructure, Mobility, Sustainability, Energy
