#  Plastic Cover Mapping - GeoAI 2024

Detecting plastic-covered cropland using satellite imagery with limited labeled data. Developed for the FAO GeoAI 2024 Challenge using region-wise stacking classifiers.

---

##  Dataset

- Satellite image tiles and labels from April–May
- Regions: Kenya, Spain, Vietnam

---

##  Methodology

- Preprocessing with `rasterio`, `numpy`, `pandas`
- Feature extraction from image bands
- Stacking Classifier using:
  - Random Forest
  - Gradient Boosting
  - Logistic Regression

---

##  Performance

- **Cross-validation Accuracy:** 99.43%
- **Metrics Used:** Precision, Recall, F1-Score (`classification_report` from `sklearn`)
- Tested on combined training data from all three regions
