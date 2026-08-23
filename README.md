# Multiview Visualisation of Leeds Road Traffic Accidents
**Live Dashboard:** [Click here](https://elizasarwat.github.io/leeds-road-accident-visualisation/)
**MSc Information Visualisation | University of Glasgow | March 2026**

Interactive exploration of 2016 Leeds road traffic accidents using three linked dashboard systems built in Python and Altair.

---

## Demo Video
[Watch the full 5-minute demo on YouTube](https://youtu.be/A-fbLzBRli0)

---

## Project Overview

This project builds three distinct interactive dashboard systems (A, B, C) to explore spatial, temporal, and environmental patterns in 1,926 road accidents across Leeds in 2016.

Each system supports three core analysis tasks:
- **T1** — Explore accident hotspots by location
- **T2** — Discover accident patterns by time of day and day of week
- **T3** — Filter a subset and summarise accident severity

---

## Systems

### System A — Spatial Exploration (Map-Centric)
- Primary view: scatter map coloured by severity (Slight / Serious / Fatal)
- Linked views: Weekday × Hour heatmap + severity bar chart
- Interaction: bidirectional brushing between map and heatmap
- File: `system_A.ipynb`

### System B — Temporal Exploration (Period-Centric)
- Primary view: donut chart showing time-of-day periods (Night, Morning Rush, Daytime, Evening Rush, Late Evening)
- Implements **generalised selection**: one click on a period filters all linked charts
- Linked views: hour bar chart + map + severity chart
- File: `system_B.ipynb`

### System C — Condition-Centric Exploration
- Primary view: road surface condition bar chart + stacked area chart
- Map acts as a bidirectional hub — brushing the map updates condition and time charts simultaneously
- Highest user satisfaction: 4.6/5 in evaluation
- File: `system_C.ipynb`

---

## Dataset

**2016 Leeds Road Traffic Accidents**
- Source: [Kaggle](https://www.kaggle.com/datasets/thedevastator/leeds-road-traffic-accidents-2009-2018)
- 1,926 accident records with spatial coordinates, time, severity, road surface, and lighting conditions
- File: `traffic_road_accident.csv`

---

## Tech Stack

| Tool | Use |
|------|-----|
| Python | Data processing and dashboard logic |
| Pandas | Data cleaning and transformation |
| Altair / Vega-Lite | Interactive visualisation |

---

## User Evaluation Results

45 task executions across 5 participants (3 tasks × 3 systems):

| System | Best For | Avg Time | Error Rate | Satisfaction |
|--------|----------|----------|------------|--------------|
| A (Spatial) | T1 — Finding accident hotspots | 28s | 0% | 4.0/5 |
| B (Temporal) | T2 — Identifying time patterns | 25s | 0% | 4.2/5 |
| C (Condition) | T3 — Multi-condition filtering | 32s | 0% | 4.6/5 |

---

## How to Run

```bash
pip install altair pandas
```

Open any notebook and run all cells:
```bash
jupyter notebook system_A.ipynb
jupyter notebook system_B.ipynb
jupyter notebook system_C.ipynb
```

Make sure `traffic_road_accident.csv` is in the same directory.

---

## My Contribution
- Implemented System A (spatial map dashboard with bidirectional brushing)
- Produced and uploaded the demo video
- Contributed to system integration and testing

---

## Team
Group 16 — University of Glasgow, COMPSCI5099 Information Visualisation 2025-26
