# Digital Photogrammetry



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
│  └─ (data files: .tif, .jpg, ...)
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

6. Push:
   ```bash
   git push -u origin main
   ```
