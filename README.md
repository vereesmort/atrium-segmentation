## Heart Segmentation
## Preprocessing Pipeline

 (`Preprocessing.ipynb`) for preprocessing heart MRI datasets for heart segmentation tasks. The workflow is built around the Medical Segmentation Decathlon (MSD) - Task02_Heart dataset.

### 📋 Overview
1.  Data Extraction: Extracts MRI image and label data from a `.tar` archive.
2.  Path Management: `pathlib` to organize and access image (`imagesTr`) and label (`labelsTr`) directories.
3.  Data Loading: Loads NIfTI (`.nii.gz`) files using `nibabel` for 3D medical imaging.
4.  Visualization: Visualizes MRI slices and segmentation masks with `matplotlib`.
5.  Preprocessing: Includes helper functions to:
    -   Map image files to corresponding label files
    -   Normalize and prepare data arrays  
    -   Optionally resize or crop image volumes for model input

### Dataset
- **Source:** [Medical Segmentation Decathlon (MSD)](http://medicaldecathlon.com/) - Heart dataset
- **Type:** 3D Semantic Segmentation
- **Format:** NIfTI
```
Task02_Heart/
├── imagesTr/
│   ├── la_001.nii.gz
│   ├── la_002.nii.gz
│   └── ...
└── labelsTr/
    ├── la_001.nii.gz
    ├── la_002.nii.gz
    └── ...
```
