# Data

The raw data is **not stored in this repository** because it is about 4.5 GB, which exceeds GitHub's file size limits.

## Source

We use the MATR dataset (Severson et al., 2019; Attia et al., 2020) in the standardized format released by **BatteryLife** (Tan et al., KDD 2025).

- BatteryLife processed data (Zenodo): https://zenodo.org/records/14969822 (see the record page for the latest version)
- BatteryLife code repository: https://github.com/Ruifeng-Tan/BatteryLife
- Original MATR data: https://data.matr.io/1/projects/5c48dd2bc625d700019f3204

Download these two files from the Zenodo record:

- `MATR.zip` (one `.pkl` file per battery, 169 batteries)
- `Life labels.zip` (cycle-life label for each battery)

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

For a Google Colab run you do not need this folder: put the two zip files in `MyDrive/CHE1147/` on Google Drive and the notebook unzips them automatically.
