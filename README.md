# IELE756 – Migration, Health, and Socioeconomic Integration in Chile.
Team members:
- Catalina Cornejo
- Javiera García

Comunas: Renca, Lo Barnechea, Buin.

Description: This repository contains the work developed for IELE756 – Preparación y Análisis de Datos. The project analyzes migration, health outcomes, and socioeconomic integration in Chile using Census 2024, ENO, and GRD datasets.

The final project builds on Tareas 0, 1, 2, and 3, but focuses on one specific anomaly identified during the previous tasks instead of summarizing the full pipeline again. The objective is to isolate, explain, and defend this finding using data already processed in earlier stages of the project.

## Final project anomaly

The selected anomaly is the over-representation of foreign patients in obstetric hospitalizations in the GRD data.

Across Renca, Lo Barnechea, and Buin, foreign patients represent a relatively small share of total hospital discharges and of the total population. However, within ICD-10 Chapter 15, pregnancy, childbirth, and the puerperium, their share is substantially higher. This is surprising because we would have expected the foreign share in obstetric hospitalizations to be closer to their overall share in the GRD data or to their population share across the selected comunas.

## Main notebook

The final project notebook is:

`notebooks/final_anomaly.ipynb`

This notebook produces the headline figure used in the video and runs the checks used to evaluate alternative explanations for the anomaly. It uses pre-computed CSV outputs from the previous tasks instead of re-running the full original pipeline.

Approximate running time: [write running time here].

## How to run

Install the required dependencies:

```bash
pip install -r requirements.txt

