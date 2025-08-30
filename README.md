# Tooth Detection using YOLO
This repository provides an end-to-end pipeline for *tooth detection* using YOLO models. It includes dataset handling, training workflows, inference, and experiment artifacts to reproduce and improve results.

---

## Project Structure
TOOTH_DETECTION/
├── dataset/              # Raw tooth dataset  
├── dataset_split/        # Train/val/test split files  
├── experiments/          # Experiment configurations & logs  
├── outputs/              # Model outputs and metrics  
├── runs/                 # YOLO training runs (checkpoints, metrics)  
├── tooth_detection.ipynb # Interactive notebook for training & inference  
├── requirements.txt      # Python dependencies  
├── pyproject.toml        # Project setup/configurations  
└── .gitignore            # Files excluded from version control  

---

## Quick Start Guide
### 1. Clone the repo
git clone https://github.com/Prakhar1230/Tooth_detection.git  
cd Tooth_detection  

### 2. Install dependencies
Create a virtual environment:  
python -m venv venv  
# On Unix/macOS:  
source venv/bin/activate  
# On Windows:  
venv\Scripts\activate  

Install required packages:  
pip install -r requirements.txt  

### 3. Explore the dataset
Set up training/validation splits if needed using `dataset_split/`. Verify the formats (e.g., image annotations, folder structure).

### 4. Train a YOLO model via the notebook
Open the interactive notebook:  
jupyter notebook tooth_detection.ipynb  

Run cells to:  
- Load the dataset.  
- Configure model and training hyperparameters.  
- Train the model and view metrics.  

### 5. Inspect training output & inference
Model artifacts, metrics, and logs are saved under `runs/`, `experiments/`, and `outputs/`. Visualize training progress using tools like TensorBoard if available.

---

## Notes & Tips
- Large weight files (`.pt`) are excluded via `.gitignore` to keep the repo clean.  
- Use the notebook as your main workflow driver — it includes reproducible steps and structure for collaboration.  
- For future versions, consider:  
  - Adding dataset download scripts,  
  - Integrating Docker for environment consistency,  
  - Adding evaluation scripts with metrics and visualization.  

---
