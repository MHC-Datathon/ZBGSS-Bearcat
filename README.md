# 🚍 NYC Bus Violation Impact Analysis
## 📖 Project Overview

- This project was developed as part of the MHC++ Datathon, a competition focused on data-driven solutions to real-world problems. Our team analyzed MTA Bus Automated Camera Enforcement (ACE) violation data and bus speed data to understand how different types of traffic violations impact travel times and delays.

## 🏙️ Background

- The Automated Camera Enforcement (ACE) program is used by the MTA to monitor traffic violations that disrupt bus operations. ACE cameras automatically detect vehicles committing violations and issue fines.

- Initial Fine: $50 for a first violation

- Uniform Fines: All violations result in the same penalty, regardless of impact.

- Main Violation Types:

  - Bus lane violations – vehicles blocking or driving in bus-only lanes.

  - Bus stop violations – vehicles obstructing designated bus stops.

  - Double parking violations – vehicles blocking traffic by parking illegally alongside another vehicle.

## ❓ Research Questions

- Should all fines cost the same amount?

- Do some violations affect travel time more than others?

## 📊 Datasets

We combined violation data with bus route segment travel times to measure the effect of traffic violations on average travel time.

- [MTA Bus Automated Camera Enforcement Violations: Beginning 2019](https://data.ny.gov/Transportation/MTA-Bus-Automated-Camera-Enforcement-Violations-Be/kh8p-hcbm/data_preview)

  - Contains records of traffic violations (bus lane, double parked, bus stop blockages) captured by ACE cameras dating back to 2019.

- [MTA Bus Route Segment Speeds: Beginning 2025](https://data.ny.gov/Transportation/MTA-Bus-Route-Segment-Speeds-Beginning-2025/kufs-yh3x/data_preview)

  - Historical dataset of bus segment speed and travel times for 2025.

- [MTA Bus Route Segment Speeds: 2023–2024](https://data.ny.gov/Transportation/MTA-Bus-Route-Segment-Speeds-2023-2024/58t6-89vi/about_data)

- Historical dataset of bus segment speeds and travel times for 2023–2024.

## 🛠️ Methods

- Tools Used:

  - Python (Pandas, NumPy, Matplotlib, Seaborn)

  - Jupyter Notebook for analysis

  - Microsoft PowerPoint for presenting findings

- Steps:

  - Cleaned and merged datasets by stop ID, route, date, and hour.

  - Computed average travel times across segments for each violation type.

  - Built bar charts and a pie chart in Python to visualize violation frequency and impact.

  - Designed a PowerPoint presentation to communicate insights and recommendations.

## 🔑 Key Findings

- Bus lane violations added about 5 minutes per segment at certain violation counts, making them the most impactful violation type. While this may seem small, it is important to remember these times represent the travel time between any two stops along the bus route. When repeated across multiple segments, delays can compound into significant lost time for each full route.


- Even small per-segment delays compound across full bus routes, affecting thousands of riders daily.

- Current fines ($50 first offense) are uniform, but findings suggest some violations (like bus lane blockages) have disproportionately higher impacts — raising the question of whether fines should vary by violation type.

## ⚠️ Limitations

- The analysis could not fully isolate each violation type by holding the other two at zero. For example, bus-lane violations were not measured independently of bus-stop and double-parked violations, so overlap may influence the observed delays.

## 💡 Business Recommendations

- Reevaluate Fine Structures: 

  - Consider differentiated fines that reflect the severity of travel time impact.

- Public Communication Campaigns:

  - Share statistics with the public showing how violations slow buses for thousands of riders.

  - Example message: “Bus lane violations have the potential to double travel time for NYC buses.”

- Deterrence Campaigns:

  - Highlight fines and reinforce enforcement efforts.

  - Use data-driven messaging to shift driver behavior.

## 📈 Visuals

- Bar chart: violation counts vs. average travel time per segment.

- Pie chart: proportion of violations by type.

- Selected charts integrated into a PowerPoint slide deck for final presentation.

## 📂 Repository Contents

This repository includes all files developed and submitted for the MHC++ Datathon:

1. MHC++ Datathon Project.ipynb
    - Jupyter Notebook containing all Python code used for cleaning, merging, and analyzing the datasets, as well as generating charts.

2. MHC++ Datathon Presentation Slides.pdf
    - Full presentation slides used during the datathon, including visuals, key findings, and recommendations.

3. MHC++ Datathon Condensed Video Presentation.mp4
    - A short video summarizing the project, where the team explains the analysis and findings using a condensed version of the slides.
  
## 🧠 Lessons Learned

1. Understand the dataset deeply by studying the data dictionary 

    - Use the data dictionary to confirm exactly what each column represents (definitions, units, valid values).

2. Don’t get stuck on one idea

    - Be willing to pivot from you original idea or ask new questions as patterns emerge. An iterating process allows for clearer research questions and more actionable findings.

## 🚀 Next Steps

- Develop a pricing model to adequately match fine amounts to the level of delay each violation type causes for NYC buses.

- Create communication and deterrence campaigns to inform citizens how violations can slow down buses for thousands of NYC riders
