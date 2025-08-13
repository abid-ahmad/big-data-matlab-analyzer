# 📊 MATLAB Interactive Big-Data Analysis

A MATLAB program that loads a **large dataset (≥ 2,000 rows)** and lets a user interactively explore, clean, analyze, visualize, and **fit regression curves**—all from a simple, menu-driven interface. Built for **BE 1500 (Fall 2024) — Extra Credit Project**.

---

## 📌 Overview
- **Automatic data loading** from `/data`.
- **Menu UI** for choosing operations (no code edits required).
- **User-defined functions (UDFs)** for analysis, visuals, and utilities.
- **End-to-end workflow:** describe → filter/sort → analyze → visualize → fit curve → export results.

---

## ⚙️ Features (what the program can do)
- **Descriptive statistics:** mean, median, std, min/max, percentiles, IQR.
- **Sort & filter:** by any column; logical indexing & thresholds.
- **Derived columns:** simple transforms (e.g., normalize, z-score).
- **Comparisons:** group-by summaries (e.g., category averages).
- **Visualizations (at least two):**
  - 2D plots (line/scatter)
  - 3D scatter/surface (if applicable)
  - Histograms
  - Bar/Pie charts
  - Tables (printed neatly to console / file)
- **Curve fitting / regression:** linear or polynomial fit with R².
- **Export:** figures (`/results/figures`) and CSV summaries (`/results/tables`).

---

## 🧱 Architecture (meets assignment requirements)
- **Main script:** `main_script.m`
  - Loads dataset automatically from `/data`.
  - Presents a **menu** of tasks and loops until the user exits.
  - Calls all user-defined functions.
- **User-defined functions (≥ 2)**
  - Example (actual filenames may differ):
    - `compute_descriptives.m` – stats
    - `sort_by_column.m` – sorting
    - `filter_by_rule.m` – logical indexing
    - `plot_histogram.m`, `plot_scatter2d.m`, `plot_bar.m` – visualizations
    - `fit_linear_regression.m` – curve fitting
  - Each function has **input & output arguments** and uses at least one of:
    - `if/else`, `switch/case`, `for/while` loops, or **nested loops**.

---

## 🗂 Repository Structure
