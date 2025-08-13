# 📊 MATLAB Interactive Big-Data Analysis (COVID-19 Dataset)

A MATLAB project that loads a **large dataset (≥ 2,000 rows)** and lets the user interactively **explore, analyze, visualize, and fit regression curves** — all from a simple, menu-driven interface.  
Built for **BE 1500 (Fall 2024) — Extra Credit Project**.

---

## 📌 Overview
- **Automatic dataset loading** from `covid_dataset.csv` (or `covid_dataset.xlsx`)
- **Interactive menu UI** — no manual code edits required
- **Modular user-defined functions** for stats, prediction, visualization, and regression
- **End-to-end workflow:** describe → predict → visualize → fit curve → (optionally) export

---

## ⚙️ Features

### 1) Descriptive Statistics
Calculates:
- **Total** new cases  
- **Mean** new cases (handles missing values)  
- **Min / Max / Range** of new cases

> Output is printed neatly to the MATLAB Command Window.

### 2) Trend Prediction
Simple signal-based prediction using historical averages:
- **Average New Cases (Overall)**
- **Predicted New Cases (Next Day)**
- **Average New Deaths (Overall)**
- **Predicted New Deaths (Next Day)**

### 3) Visualization
Generates multiple plots to explore trends:
- **2D Line Plot:** New COVID-19 cases over time  
- **Bar Chart:** New deaths over time  
- **3D Scatter:** Cases vs. deaths vs. days

### 4) Regression Curve Fitting
- Fits a **linear regression** to COVID-19 cases vs. time  
- Overlays **actual vs. fitted** line on the same plot (with legend, labels, and grid)

---

## 🧱 File Architecture

| File | Purpose |
|---|---|
| `main.m` | **Entry point** — loads data and shows the interactive menu |
| `descriptive_stats.m` | Computes total, mean, min, max, and range of new cases |
| `predict_model.m` | Computes overall averages and **next-day** predictions |
| `visualize_results.m` | Creates **2D**, **bar**, and **3D** plots |
| `fit_regression_curve.m` | Fits and plots a **linear regression** curve |
| `covid_dataset.csv` (or `covid_dataset.xlsx`) | COVID-19 dataset used by the program |

## 📄 Documentation (included in this repo)

- [**Project_Instructions.pdf**](report/Project_Instructions.pdf) — How to run the project and what each menu option does.  
- [**Project_Code.pdf**](report/Project_Code.pdf) — Full MATLAB code listing for review.  
- [**Project_Results.pdf**](report/Project_Results.pdf) — Sample outputs, plots, and brief discussion of results.

---

## ▶️ How to Run
1. **Download the project archive**  
   - Click here to download: [📦 MATLAB_Regression_Project_BE1500.zip](report/MATLAB_Regression_Project_BE1500.zip)  
   - Extract the contents to a location on your computer.

2. **Organize the files**  
   - Ensure **all extracted files remain together** in a single folder (do not move or rename individual files).  
   - The folder structure should match what’s provided in the `.zip` file.

3. **Open in MATLAB**  
   - Launch MATLAB.  
   - In the **Current Folder** panel, navigate to the extracted project folder.  
   - Alternatively, use:
     ```matlab
     cd('path_to_extracted_folder')
     ```

4. **Run the main script**  
   - Locate the main file (e.g., `main.m`) in MATLAB’s file browser.  
   - Press the **Run** button or type:
     ```matlab
     main
     ```

5. **Follow the menu prompts**  
   - The program provides an interactive menu for data exploration, visualization, and regression analysis.
