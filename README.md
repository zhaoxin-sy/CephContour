##  CephContour: A Multi-Center Dataset and Contour-Guided Multi-Task Cephalometric Diagnosis
Cephalometric diagnosis plays a pivotal role in orthodontics. Currently, the dominant landmark-based "detect-then-measure" pipelines are inherently hindered by error accumulation. 

To bypass landmark regression and alleviate structural ambiguity, we construct **CephContour**, a multi-center dataset comprising 2,000 lateral cephalograms. This dataset standardizes six clinical diagnostic tasks based on ABO standards. More importantly, it provides **expert-annotated dense cephalometric tracings**, enabling a novel contour-aware learning paradigm. 

Leveraging this dataset, our proposed Contour-Guided Multi-Task Framework achieves **93.51% average accuracy** and **98.75% AUC**, establishing a new state-of-the-art.

---

## Datasets
To demonstrate the high quality of our data format and expert annotations during the review phase, we provide a **sample subset** (3 representative de-identified patients) in the `sample_data/` directory:

```text
Dataset/
├── images/                  # Raw lateral cephalograms (.png)
├── tracings/           # Expert-annotated dense structural tracings (.png)
└── labels.txt        # Diagnostic classifications for the 6 tasks
