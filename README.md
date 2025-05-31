# Exploring the P300 in EEG Data  
**Fa Ojeda – Brainhack School 2025**

This project explores how the brain responds to salient auditory and visual stimuli using EEG data from the MNE sample dataset. The focus was on extracting and visualizing the **P300** component — a well-known event-related potential (ERP) associated with attention and stimulus evaluation.

---

## Objective

To build foundational skills in EEG preprocessing, event segmentation, and ERP analysis using open neuroimaging tools. Special emphasis was placed on identifying the P300 response under different stimulus conditions, as a precursor to future studies on emotional modulation.

---

## Dataset & Tools

- **Dataset**: [MNE Sample Dataset](https://mne.tools/stable/overview/datasets_index.html#sample-dataset) (auditory/visual oddball task)
- **Tools**: MNE-Python, Jupyter Notebook
- **Conditions compared**:  
  - Event 2: Right auditory tone (frequent – "standard")  
  - Event 5: Visual face stimulus (rare – "deviant")

---

## Analysis Workflow

1. Load EEG data and select EEG-only channels  
2. Apply band-pass filter (1–40 Hz)  
3. Set electrode montage (10-20 layout, where possible)  
4. Detect events and define experimental conditions  
5. Create epochs time-locked to stimulus onset (−200 ms to +800 ms)  
6. Compute and plot:
   - ERP waveforms for each condition
   - Difference wave (deviant – standard)
   - (Topomap visualization was attempted, but limited by dataset constraints)

---

## Results

- A clear **P300-like positive deflection** was observed around 300 ms in both conditions.
- Contrary to expectations, the P300 amplitude was **slightly higher in the "standard" condition**.
- The **difference wave** showed modest divergence, suggesting the rare visual stimulus was not sufficiently salient to drive a robust P300.
- Topographic maps could not be accurately computed due to the use of generic EEG channel names (`EEG 001`, `EEG 002`, etc.) in the dataset.

---

## Interpretation

Although the deviant stimulus (a rare visual face) was expected to elicit a larger P300, the results suggest that **stimulus rarity alone** may not be enough — perceptual and emotional salience are also critical. This highlights the importance of thoughtful stimulus design in ERP research.

---

## Conclusion

This project successfully demonstrated the full EEG analysis pipeline for extracting ERPs and visualizing the P300. The skills gained here will be directly applicable to future work using **emotionally salient stimuli** and more carefully controlled designs.

---

## Files

- `P300_EEG_Analysis.ipynb`: Jupyter Notebook with code and results
- `figures/`: Contains exported plots (optional)
