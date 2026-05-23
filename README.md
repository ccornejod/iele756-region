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

Approximate running time: 5–10 minutes, depending on the local machine.

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

The notebook regenerates the headline figure and the supporting checks used in the final video.

## Final video

The video link is included in the opening Markdown cell of:

```text
notebooks/final_anomaly.ipynb
```

## AI-use disclosure

We used ChatGPT as an assistant during the project. It helped us organize the structure of `final_anomaly.ipynb`, debug Python code, improve Markdown explanations, and prepare the video script.

The AI tool was not used as a data source. All calculations were produced from our notebooks and datasets, and all numerical results, figures, and interpretations were reviewed by the team. We remain responsible for every claim, number, and file included in this repository.
