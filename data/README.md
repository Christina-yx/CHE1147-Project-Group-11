# Data

The raw data is **not stored in this repository** because it is about 4.5 GB, which exceeds GitHub's file size limits.

## Option 1 (recommended): exact copy used in this project

The two files we used, `MATR.zip` and `Life labels.zip`, are shared in this Google Drive folder:

**https://drive.google.com/drive/folders/1TNz7eRyQK8LhgMinQf1B7XcOt19_b6eg?usp=sharing**

Using this copy guarantees the same data as in our report.

- **To run in Google Colab:** open the link, then right-click the `CHE1147` folder → **Organize → Add shortcut** → choose **My Drive**. The notebook then finds the files at `MyDrive/CHE1147/`. (Alternatively, download the two zip files and upload them to a folder `MyDrive/CHE1147/` in your own Drive.)
- **To run locally:** download both zip files and unzip them into this `data/` folder (see the layout below).

## Option 2: original source

We use the MATR dataset (Severson et al., 2019; Attia et al., 2020) in the standardized format released by **BatteryLife** (Tan et al., KDD 2025). The same two files can be downloaded from the BatteryLife Zenodo record:

- BatteryLife processed data (Zenodo): https://zenodo.org/records/14969822 (several versions exist; for exact reproduction use the Google Drive copy above)
- BatteryLife code repository: https://github.com/Ruifeng-Tan/BatteryLife
- Original MATR data: https://data.matr.io/1/projects/5c48dd2bc625d700019f3204

## Expected layout for a local run

Unzip both files into this `data/` folder so that it looks like this:

```
data/
├── MATR/
│   ├── MATR_b1c0.pkl
│   ├── MATR_b1c1.pkl
│   └── ...            (169 files)
└── Life labels/
    └── MATR_labels.json
```

For a Google Colab run you do not need this folder: the notebook unzips the files from `MyDrive/CHE1147/` automatically.
