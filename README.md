# 🏀 WNBA Spatial Gravity & Predictive Scouting

**Live Interactive Demo:** [View the Dashboard Here](https://noushinh.github.io/wnba-predictive-scouting/)

## Executive Summary
This project is an interactive sports analytics web application built with Python, Dash, and Plotly. It processes **real WNBA spatial tracking data** from actual games to model **Defensive Gravity**—a player's ability to draw defensive attention and generate floor spacing for teammates. 

The dashboard benchmarks actual observed defensive pull against a Machine Learning-predicted baseline (xGrav) to identify high-value spacing threats on the court.

## 📌 Core Features
* **Predictive ML Engine (xGrav):** Utilizes a Scikit-Learn `RandomForestRegressor` to predict expected defensive attraction based on coordinate geometry, distance to the rim, and game time.
* **Spatial Court Footprints:** Parses real tracking centroids into float coordinates, generating dynamic court overlays to visualize a player's active attention radius and defender swarm.
* **Game-Minute Heatmaps:** Aggregates real, high-frequency WNBA tracking telemetry into 40-minute regulation matrices to track defensive attention fluctuations over the course of a game.
* **Educational Simulator:** A configurable "What-If" modeling tool teaching how defensive collapses (single coverage vs. double-team traps) impact overall gravity scores across different threat zones (Perimeter, Mid-Range, Paint).

## 🛠 Technical Stack
* **Language:** Python
* **Frontend UI:** Dash, Dash Bootstrap Components (`LUMEN` theme)
* **Data Visualization:** Plotly Graph Objects, Matplotlib, Seaborn
* **Data Processing:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn

## 🔒 Data Governance & Privacy Note
*Please note: The underlying high-frequency optical tracking telemetry used to train these models is real, proprietary WNBA game data. To strictly adhere to data privacy and sports analytics sharing guidelines, the raw CSV tracking files have been omitted from this public repository. The linked HTML export above serves to demonstrate the analytical architecture, visual outputs, and interactive UI of the final application using the real dataset.*
