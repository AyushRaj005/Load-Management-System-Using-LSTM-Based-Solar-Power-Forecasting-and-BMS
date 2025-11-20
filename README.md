# Load Management System using LSTM-Based Solar Power Forecasting and BMS  
_A Minor Project by Ayush – 6th Semester, NIT Meghalaya_

## Project Overview  
This project addresses the design and implementation of an integrated renewable energy system for small-scale industry or institute use. The system combines:

- Solar power forecasting using advanced machine learning (especially Bi-LSTM) and weather data  
- Battery Management System (BMS) for state-of-charge (SOC) and state-of-health (SOH) prediction  
- Optimisation and control of load management to maximise renewable usage and battery longevity  

The goal is to build an economical, efficient, and safe integrated model of solar generation + forecasting + battery system, culminating in a MATLAB/Simulink model for practical implementation.

## Motivation  
With the ever-increasing push toward renewable energy, solar power systems are becoming more ubiquitous. However, challenges still exist:

- Variability in solar generation due to weather fluctuations  
- Battery degradation and management risks  
- Need for predictive models for better utilisation of resources  

By forecasting solar power output accurately and integrating a smart BMS alongside load management, this project aims to improve system reliability, efficiency, and cost-effectiveness.

## Project Scope & Objectives  
### Objectives  
1. Collect historical solar generation and weather data and preprocess it.  
2. Develop a forecasting model (Bi-LSTM and other candidate ML methods) for solar power output.  
3. Model battery behaviour: Predict SOC & SOH under varying loads/conditions.  
4. Design a load management strategy: matching load demand, solar supply, and battery support.  
5. Build a MATLAB/Simulink model to simulate the total system and evaluate performance (e.g., energy utilisation, battery cycling, cost savings).  
6. Analyse results, validate forecasting and battery models, and highlight potential deployment considerations for small-scale industries or institutes.

### Scope  
- System scaled to small industrial/institutional loads rather than large utility scale  
- Use of publicly available weather data and solar generation datasets  
- Emphasis on forecasting accuracy, battery health prediction, and practical integration  
- Simulink model serves as demonstration rather than full physical implementation  

*Note: adjust actual paths/files if different in your repo.*

## Installation & Setup  
1. Clone the repository:  
   ```bash
   git clone https://github.com/AyushRaj005/Load-Management-System-Using-LSTM-Based-Solar-Power-Forecasting-and-BMS.git
   cd Load-Management-System-Using-LSTM-Based-Solar-Power-Forecasting-and-BMS
````

2. Create and activate a Python virtual environment (recommended):

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # Mac/Linux
   # On Windows: venv\Scripts\activate
   ```

3. Install required Python packages:

   ```bash
   pip install -r requirements.txt
   ```

4. For Simulink: Open MATLAB and load the `simulink/` folder models. Ensure you have the required toolboxes (e.g., Simulink, Control System, Stateflow) installed.

5. Configure data paths / settings in `src/config.py` (or equivalent) to point to your `data/` folder.

### Simulink Simulation

1. Open MATLAB and load `simulink/main_system.slx`
2. Adjust simulation parameters (time-step, load profile, solar generation profile)
3. Run the simulation and view results in `results/` folder

## Evaluation & Results

* Solar forecasting results: Accuracy metrics (MAE, RMSE, R²) for Bi-LSTM and baseline models.
* Battery SOC/SOH prediction: Error metrics and health degradation curves.
* System simulation: Load vs generation vs battery usage graphs, efficiency metrics, cost savings estimation.
* Detailed discussion available in the full report (see `minor_proj.pdf`).

## Key Insights & Learnings

* Accurate forecasting reduces battery cycling and ensures better utilisation of solar generation.
* Battery health prediction is crucial for long-term viability and cost-effectiveness.
* System integration is non-trivial: mismatches between generation/load and real-time control are major losses.
* Simulation results suggest potential for small-scale deployment with appropriate design and forecasting fidelity.

## References

For full theory, models, and implementation details, please refer to the project report: [minor_proj.pdf](minor_proj.pdf).

