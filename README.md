# IELE756 – Final Project: One Anomaly, Defended

## Team members

- Catalina Cornejo
- Javiera García

## Selected comunas

- Renca
- Lo Barnechea
- Buin

## Anomaly

The selected anomaly is the over-representation of foreign patients in obstetric hospitalizations in the GRD data.

Across Renca, Lo Barnechea, and Buin, foreign patients represent 6.68% of all GRD hospital discharges. However, within ICD-10 Chapter 15, which corresponds to pregnancy, childbirth, and the puerperium, their share rises to 19.69%.

This is surprising because the foreign-patient share in obstetric hospitalizations was expected to be closer to the overall GRD baseline or to the demographic weight of foreign-born residents in the selected comunas. Instead, the observed share in Chapter 15 is almost three times the overall GRD baseline.

## Main notebook and headline figure

The final project notebook is:

```text
notebooks/final_anomaly.ipynb
```

This notebook produces the headline figure used in the video and contains the code used to isolate and defend the anomaly.

The headline figure is saved as:

```text
figs/headline.png
```

Approximate running time: 5–10 minutes, depending on the local machine, when using the prepared project files.

## Data files used by the final notebook

The final notebook is organized around prepared project outputs, so the main anomaly analysis can be reproduced without re-running the full raw GRD pipeline.

The files needed for the final analysis are:

```text
census_team20.csv
grd_team20.csv
chapter_nat_summary.csv
```

The file `chapter_nat_summary.csv` is an intermediate summary created from the GRD raw files. The notebook includes the code used to generate this file from the large GRD ZIP files, but the final anomaly analysis uses the prepared CSV summary to keep the project reproducible and focused.

The large raw GRD ZIP files are not committed to the repository, following the project instructions. If a user wants to re-create `chapter_nat_summary.csv` from the raw data, the following files must be placed in the project directory before running that section of the notebook:

```text
GRD_PUBLICO_2022.zip
GRD_PUBLICO_2023.zip
GRD_PUBLICO_2024.zip
CIE-10.xlsx
```

## How to install dependencies and run the notebook

Clone the repository:

```bash
git clone https://github.com/ccornejod/iele756-region.git
```

Enter the repository folder:

```bash
cd iele756-region
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Open Jupyter Notebook or JupyterLab:

```bash
jupyter notebook
```

or:

```bash
jupyter lab
```

Then open and run:

```text
notebooks/final_anomaly.ipynb
```

The notebook regenerates the headline figure and the supporting checks used in the final video from the prepared project files.

## Final video

The video link is included in the opening Markdown cell of:

```text
notebooks/final_anomaly.ipynb
```

## AI-use disclosure

We used ChatGPT as an assistant during the project. It helped us organize the structure of `final_anomaly.ipynb`, debug Python code, improve Markdown explanations, prepare the video script, and improve the README wording.

The AI tool was not used as a data source. All calculations were produced from our notebooks and datasets, and all numerical results, figures, and interpretations were reviewed by the team. We remain responsible for every claim, number, and file included in this repository.
