# CIVE202_Project5 - Kiewit Corporation

This repository contains the files and information for CIVE 202 Project #5. The Python code in this project is used to automate steel design calculations for a W-shaped tension member based on AISC Example D.1. The purpose of this project is to help Kiewit Corporation standardize steel tension member calculations instead of relying on individual Excel spreadsheets that may not all function the same way. For this project, the code checks tensile yielding, tensile rupture, and slenderness. The code also uses LRFD and ASD design values to compare the required strength with the available strength. Three different W-shape scenarios are analyzed in the project: W8x21, W10x33, and W6x15. The results are then put into tables and plotted to compare the different steel sections. The project uses Python packages such as pandas, numpy, matplotlib, and steelpy. The steelpy package is used to pull W-shape and WT-shape properties instead of hardcoding all the values by hand.

# Repository Contents

- Project_5.ipynb – Main Python notebook for the project

- Project_5.py – Python script version of the project code

- Project5_AnnotatedCode.docx – Document with explanations of the Python code

- Project-5_Final_Report.docx – Final report explaining the methods, results, and discussion

- Project 5 Scope of Work.docx – Scope of Work laying out the client request, tasks, and deliverables

- Project5Gantt.xlsx – Gantt chart showing the project schedule

- Project5_Timesheet.xlsx – Timesheet showing the team’s hours spent on each activity

- README.md – Summary of the project and instructions for running the code

# How To Run

To run the code, first download the Python notebook to your device. Open the notebook in Jupyter Notebook or JupyterLab. The main packages used in this project are pandas, numpy, matplotlib, and steelpy. If steelpy is not already installed, run the install line in the notebook or use: pip install steelpy. After the packages are installed, run each cell in the notebook from top to bottom. The first section imports the required packages and sets up the constants used in the calculations. The next section loads the W-shape and WT-shape section properties from steelpy. After that, the code defines the functions used for tensile yielding, tensile rupture, slenderness, and the full tension member design check. The final sections run the three scenarios and create the LRFD and ASD comparison plots.

# User Guide

The Python notebook is the main file that runs the project calculations. The annotated code document explains what each major part of the code does. The written report explains the background of the project, the method used, the three scenarios, the results, and how the plots compare the different W-shapes. The code does not require raw data files because the steel section properties are pulled from the steelpy package. To change the steel section being analyzed, the user can edit the scenario inputs in the notebook. For example, a user can change the W-shape name, dead load, live load, connection length, number of bolt holes, or material properties.

The three scenarios already included in the notebook are:

Scenario 1: W8x21

Scenario 2: W10x33

Scenario 3: W6x15

The results from each scenario include the LRFD required strength, ASD required strength, available yielding strength, available rupture strength, slenderness ratio, and governing limit state. The plots are used to visually compare the required strength, yielding strength, and rupture strength for each scenario.
