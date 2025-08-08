# Digital Photogrammetry

A minimal, push-ready project containing a Jupyter notebook (**Digital_Photogrammetry.ipynb**) and a **Data/** folder where required datasets/images should be placed.

## Requirements
- Python 3.9+
- Packages listed in `requirements.txt` (NumPy, OpenCV, Matplotlib, SciPy, Pillow)

Install:
```bash
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

## Folder structure
```
Digital Photogrammetry/
├─ Data/
│  └─ (your data files: .tif, .jpg, ...)
├─ Digital_Photogrammetry.ipynb
├─ requirements.txt
├─ .gitignore
├─ .gitattributes   # enables Git LFS for TIFF files (optional, recommended for large images)
└─ LICENSE
```

> If your images are large (e.g., TIFF), enable **Git LFS** to avoid push errors:
```bash
git lfs install
git lfs track "*.tif" "*.tiff"
```

## Running the notebook
1. Put your images/data in the `Data/` folder.
2. Open `Digital_Photogrammetry.ipynb` in Jupyter/VS Code and update any file paths to point to `Data/<yourfile>`.
3. Run the cells.

## Publish to GitHub — step by step
1. Create a new repository in your GitHub account (e.g., **Digital-Photogrammetry**) under `github.com/KosarAsadii`.
2. In your terminal, go to the project folder (quotes are needed because the folder name has a space):
   ```bash
   cd "D:\KNTU\Term1\Digital Photogrammetry\Exercise\Digital Photogrammetry"
   ```
3. (Optional) Test the environment:
   ```bash
   python -m venv .venv
   .venv\Scripts\activate
   pip install -r requirements.txt
   ```
4. Initialize Git, (optionally) set up LFS, commit:
   ```bash
   git init
   git lfs install
   git add .
   git commit -m "Initial commit: Digital Photogrammetry notebook and data structure"
   git branch -M main
   ```
5. Add the remote (adjust if you chose a different repo name):
   ```bash
   git remote add origin https://github.com/KosarAsadii/Digital-Photogrammetry.git
   ```
6. Push:
   ```bash
   git push -u origin main
   ```