AGP_PIPELINE

Interpretable ML Case Study on American Gut Project data

Data DOI: https://doi.org/10.5281/zenodo.16989509

Script: agp_pipeline.ipynb
License: MIT (code); CC BY 4.0 (data)



Download these files from the Zenodo record above and keep their filenames the same:

AG_100nt_even1k.biom

10317_20250712-045924.txt (Qiita 10317 metadata; TSV)

97_otu_taxonomy.txt (Greengenes 13_8 taxonomy)

filtered_metadata.csv

filtered_otu.csv

otu_processed.csv

y_labels.csv

Quick start on Google Colab

Mount Drive:

from google.colab import drive
drive.mount('/content/drive')

In Google Drive, use: MyDrive/Colab Notebooks/

Upload all Zenodo files into that folder.

Install packages in Colab:

!pip install -q pandas numpy scikit-learn xgboost lightgbm imbalanced-learn shap biom-format h5py matplotlib seaborn


Make sure these paths in agp_pipeline.py match your Drive:

biom_fp = '/content/drive/MyDrive/Colab Notebooks/AG_100nt_even1k.biom'
meta_fp = '/content/drive/MyDrive/Colab Notebooks/10317_20250712-045924.txt'
taxonomy_path = '/content/drive/MyDrive/Colab Notebooks/97_otu_taxonomy.txt'
otu_path = '/content/drive/MyDrive/Colab Notebooks/filtered_otu.csv'
meta_path = '/content/drive/MyDrive/Colab Notebooks/filtered_metadata.csv'


Finally, run the script block-by-block in Colab.



Reproducibility notes

Fixed seed (42), stratified split, no data leakage

How to cite

Clark, S. (2025). American Gut (Qiita 10317) Inputs and Processed Tables for Affective-Disorder Microbiome ML Pipeline (v1.0) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.16989509
