# Dataset Download Instructions

Due to file size limitations on GitHub, the complete dataset used in this project must be downloaded from its official source. Follow the steps below to set up the data directory.

## Step 1: Download the Dataset
1. Visit the dataset source link: `[INSERT_URL_HERE]` (e.g., Kaggle, UCI Repository, etc.)
2. Download the data file, usually named `download.csv` or zipped as a `.zip` archive.
3. Extract the file if it is zipped.

## Step 2: Update the Project Folder Structure
Place the downloaded file directly into your local `data/` directory. Your folder structure must look like this for the notebooks to run correctly:

├── data/
│   ├── sample_data.csv          # Included in repository (for quick testing)
│   ├── download_instructions.md # This file
│   └── download.csv             # Your downloaded file (Add this)
├── notebooks/
└── README.md

## Step 3: Run the Notebooks
Once `download.csv` is placed inside the `data/` folder, the relative paths in the Jupyter Notebooks will automatically detect and load the dataset.
