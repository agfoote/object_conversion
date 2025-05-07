# Single-Cell Metadata Conversion Tools

This repository provides tools for converting single-cell data between different formats, specifically tailored for downstream integration and visualization workflows.

## 🔧 Files Included

- `h5ad_to_meta_conversion.ipynb`  
  Jupyter notebook to extract and convert metadata from a `.h5ad` file (AnnData format) into a tabular format suitable for external tools (e.g., R or Seurat).

- `meta_to_sobj_conversion.rmd`  
  R Markdown script for importing a metadata file into a Seurat object (`SeuratObject`) for further analysis or plotting in R.

## 🚀 Usage

### 1. Convert `.h5ad` to metadata
Open and run the notebook:
```bash
jupyter notebook h5ad_to_meta_conversion.ipynb
```

Ensure required Python packages are installed:
```bash
pip install scanpy pandas
```

### 2. Convert metadata to Seurat object
Open and knit the R Markdown file:
```R
rmarkdown::run("meta_to_sobj_conversion.rmd")
```

Ensure you have these R packages installed:
```R
install.packages("Seurat")
```

## 📎 Notes
- Make sure your `.h5ad` file and output metadata are in the correct working directory.
- Update file paths as needed in both scripts before running.

---
