# Project Panopticon – Intelligent Exam Proctoring

This repository contains an educational Jupyter Notebook demonstrating a machine-learning workflow for analyzing video telemetry and system-event logs.

## Files required

Place these CSV files in the same directory as `Project_Panopticon_GitHub.ipynb`:

- `video telemetry.csv`
- `system events.csv`

The notebook checks the required columns and stops with a clear error if either file is missing.

## Run locally

1. Install Python 3 and Jupyter Notebook.
2. Install the required packages:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

3. Put the notebook and both CSV files in one folder.
4. Open a terminal in that folder and run:

   ```bash
   jupyter notebook
   ```

5. Open `Project_Panopticon_GitHub.ipynb` and run the cells from top to bottom.

## Input columns

**video telemetry.csv**: `student_id`, `exam_id`, `timestamp`, `gaze_deviation`, `head_pose_angle`, `audio_level`, `suspicious`

**system events.csv**: `student_id`, `exam_id`, `timestamp`, `event_type`, `event_value`

## Important note

This is an educational prototype. Model flags are not proof of misconduct and must not be used for automatic disciplinary decisions. Evaluate on separate students or exam sessions before drawing conclusions about model performance.
