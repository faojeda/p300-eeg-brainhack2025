# Exploring the P300 in EEG Data  
**Fabiana Ojeda 歐瑩忻 – Brainhack School 2025**

This project explores the P300 event-related potential (ERP) component using EEG data from the MNE sample dataset. The goal was to extract and visualize P300 activity in response to frequent versus rare sensory stimuli, laying a foundation for future emotion-based EEG experiments.

---

## Objective

To implement an end-to-end EEG preprocessing and ERP analysis pipeline using open-source tools, and to evaluate P300 responses in a simple oddball-like paradigm.

---

## Dataset & Tools

- **Dataset**: [MNE Sample Dataset](https://mne.tools/stable/overview/datasets_index.html#sample-dataset)
- **Conditions**:
  - `standard` = Event ID 2 (frequent right auditory tone)
  - `deviant` = Event ID 5 (rare visual face stimulus)
- **Tools used**: Python, Jupyter Notebook, MNE-Python

---

## Methods

1. EEG-only data selection and filtering (1–40 Hz)
2. Event segmentation using STI 014 channel
3. Epoch creation (−200 ms to +800 ms)
4. ERP averaging for standard and deviant conditions
5. P300 visualization via:
   - ERP waveform comparison
   - Difference wave (deviant − standard)
6. (Topomaps omitted due to incompatible channel naming)

---

## Results

- A strong P300-like response was observed for the rare **deviant** condition.
- ERP comparison and difference wave confirm attentional engagement.
- Results validate the use of this dataset for training ERP analysis workflows.

---

## Interpretation

The deviant condition (a rare visual face stimulus) elicited a clear P300 component, consistent with the brain’s heightened attention to rare or salient events. This confirms the suitability of the MNE sample dataset for basic P300 exploration and supports its future use in emotionally modulated ERP research.

---

## Files

- `P300_EEG_Analysis.ipynb`: Main Jupyter Notebook
- `figures/erp_comparison.png`: ERP waveform comparison
- `figures/difference_wave.png`: Difference wave plot

---

## Launch Online

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/YOUR_USERNAME/YOUR_REPO_NAME/HEAD?labpath=P300_EEG_Analysis.ipynb)

---

## Author

**Fabiana Ojeda 歐瑩忻**  
Brainhack School 2025
