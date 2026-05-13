# EEG Linguistic Interference

EEG study examining how different types of background audio affect cognitive load during a listening task.

COGS 189 Final Project · UC San Diego · 2026 · Team: Five Brains

## Research Question

Does the type of background music — lyrics you understand vs. foreign lyrics vs. instrumental vs. speech — affect cognitive engagement during a task?

## Method

- 18 participants, 64-channel EEG at 512 Hz
- Four audio conditions: comprehensible lyrics, foreign lyrics, instrumental, speech
- Extracted frontal Beta (13-30 Hz) and parietal Alpha (8-12 Hz) band power
- Computed Engagement Index (Beta / Alpha ratio)
- Repeated-measures ANOVA + LOSO cross-validation

## Result

No significant condition effect (p ≈ 0.258). Classification accuracy near chance (~0.509). Simple bandpower features are likely not sensitive enough to capture linguistic interference across individuals.

## Analysis Pipeline

1. Data loading and validation
2. Experimental design verification
3. Feature extraction (Alpha / Beta band power)
4. Engagement metric computation
5. Statistical analysis and visualization

## Project Structure

eeg-linguistic/
├── notebooks/
│   ├── 01_setup_validation.ipynb
│   └── 02_feature_stats_ml_visual.ipynb
├── requirements.txt
└── README.md

## Dataset

EEG data of continuous listening of music and speech — Aalborg University:
https://vbn.aau.dk/en/datasets/eeg-data-of-continuous-listening-of-music-and-speech/

## Team

Five Brains — UC San Diego, COGS 189
