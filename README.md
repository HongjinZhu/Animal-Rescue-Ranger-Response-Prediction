# Animal-Rescue-Ranger-Response-Prediction

## Overview
This repository contains a comprehensive analysis and predictive modeling project for animal rescue response times. The project involves data preprocessing, exploratory data analysis, clustering, and predictive modeling using various machine learning techniques.

## Repository Structure
```
Animal_Rescue_Analysis/
│
├── notebooks/
│ ├── species_specific_analysis.ipynb
│ ├── temporal_trends.ipynb
│ ├── clustering_pattern_detection.ipynb
│ └── response_time_prediction.ipynb
│
└── README.md
```

## Data
The data for this project is sourced from Kaggle. Follow these steps to download the data:

1. **Install Kaggle Package**: Install the Kaggle package if you haven't already.

```bash
pip install kaggle
```

2. **Upload Kaggle API Key**:
   - Go to your Kaggle account settings (https://www.kaggle.com/account).
   - Scroll down to the "API" section and click on "Create New API Token". This will download a file named `kaggle.json`.

3. **Upload the `kaggle.json` file**: Upload the `kaggle.json` file to your project directory or Colab environment.

4. **Configure Kaggle API Key**:

```bash
mkdir -p ~/.kaggle
cp kaggle.json ~/.kaggle/
chmod 600 ~/.kaggle/kaggle.json
```

5. **Download the Dataset**:

```bash
kaggle datasets download -d mexwell/urban-park-ranger-animal-condition-response
```

6. **Unzip the Dataset**:

```python
import zipfile
import os

with zipfile.ZipFile('urban-park-ranger-animal-condition-response.zip', 'r') as zip_ref:
    zip_ref.extractall('.')

os.listdir('.')
```
