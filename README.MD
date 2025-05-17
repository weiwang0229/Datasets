# 📦 GA-HVNet Training & Evaluation Datasets

This repository contains datasets for training and testing the GA-HVNet model, covering two main problem domains:

- **HSMRTA** (Heterogeneous Service Multi-Robot Task Allocation)
- **MoTSP** (Multi-Objective Traveling Salesman Problem)

Each dataset is categorized by problem type and number of objectives (e.g. 5, 8, 10).

---

## 📁 Directory Overview

| Folder | Description |
|--------|-------------|
| `HSMRTA-DataSet-8obj/` | Dataset for the HSMRTA problem with 8 objectives |
| `MoTSP-DataSet-5obj/` | Dataset for the MoTSP problem with 5 objectives |
| `MoTSP-DataSet-8obj/` | Dataset for the MoTSP problem with 8 objectives |
| `MoTSP-DataSet-10obj/` | Dataset for the MoTSP problem with 10 objectives |

Each folder contains its own internal structure of training and test datasets.

---

## 🔍 Inside `HSMRTA-DataSet-8obj/`

This folder includes the following subfolders:

| Subfolder                               | Description                                    |
|-----------------------------------------|------------------------------------------------|
| `HSMRTA-test_folder_8obj/`              | Test set used for evaluating model performance |
| `HSMRTA-train_folder_8obj_Dataset_10k/` | Training set with 10,000 samples               |
| `HSMRTA-train_folder_8obj_Dataset_1k/`  | Training set with 1,000 samples                |

Each subfolder contains `.csv` files representing training or testing instances.

---

## 🛠️ Usage Instructions

To train the GA-HVNet model:

1. **Place the four main dataset folders in the project root directory**, like this:

    ```
    your-project/
    ├── HSMRTA-DataSet-8obj/
    ├── MoTSP-DataSet-5obj/
    ├── MoTSP-DataSet-8obj/
    ├── MoTSP-DataSet-10obj/
    └── ...
    ```

2. The internal folders (e.g. `HSMRTA-test_folder_8obj/`) are accessed directly by the training script (e.g. `Train_GA_HVNet.py`).

3. Modify your script config if you want to switch between training sets or objective settings.

---

## 💬 Notes

- All datasets are stored in **CSV format**, organized for direct loading using standard Python tools (e.g. `pandas`, `csv`, or `numpy`).
- File naming follows a clear pattern with objective count and sample count encoded in the folder name.
- No additional preprocessing is needed unless explicitly modified in the code.

---

## 📢 Citation

If you use these datasets in your research, please cite our work or mention the dataset source.
