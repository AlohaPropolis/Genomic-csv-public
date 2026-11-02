# Genomic CSV Public — Libre 3 Interstitial Glucose Variability

This repository tracks interstitial glucose variability from the business end of the Libre 3 sensor onward.

Think of this repo as a fleet: two canoes, different boats, same water.

### The Fleet — Two PDFs, Two Purposes

**1. Introduction Canoe — `Introduction-To-My-Latest-Relevant-Dataset-10-30-26.pdf` + `Libre-Intro-10-30-26.png`**
- The starting canoe — sensor setup, dataset introduction, and context from Oct 30
- How the Libre 3 data is collected, what Notes mean, and the protocol for tracking
- Read this first if you are new to the dataset

**2. Evaluation Boat — `Evaluation-GBP-Carb-Suppressor-With-Graph.pdf` (V02 perfect final)**
- The evaluation boat — focused fiber evaluation using Sensor #2
- **12-Hour Graph (Nov 1) - 89 mg/dL In Range**
- **Baseline-Matched Overlay — Corrected Legend:**
    - Orange = 5g dextrose only in 8 oz water (iAUC 657.6 mg/dL·min, peak 106)
    - Blue = 5g dextrose + 2.5g GBP in 8 oz water (iAUC 518.7 mg/dL·min, peak 92.5 adj) = **21.1% lower with GBP**
- Method: Peak 1 end baseline 87 mg/dL extrapolated to match Peak 2 end 93 mg/dL (+6.0 mg/dL linear ramp), raw data every 5 min, trapezoidal AUC
- Total AUC: 7,839.5 vs 9,195.5

### Data — The Water Both Boats Float On

- **JohnHasty_glucose_11-1-2026.csv** — Libre export, Sensor #2, 4,479 historic readings Oct 13 - Nov 1, every 5 min, 113 Notes, generated 11-02-2026 02:39 AM UTC
    - Nov 1: mean 86.1, median 87, min 67, max 106, SD 7.7
    - Acclimation Window (Hour 1-12) n=132 mean 85.5 range 67-106
    - Stable Baseline (Hour 12+) n=39 mean 88.8 range 70-100
    - Protocol: Hour 0-1 Warm-up, Hour 1-12 Acclimation Window, Hour 12+ Stable Baseline — flag don't drop
    - Key Notes: 02:35 1/2 orange + 1 tsp GBP, 04:12 Cocktail in, 10:10 5g dextrose, 11:40 Back to base, 14:54 fingersticks 58 63 66 vs sensor 69 at 14:46

### Repo Purpose
From the business end of the Libre 3 sensor onward, this repo will continue to track interstitial glucose variability — new datasets, new evaluations, same transparent method.

**Author:** John Hasty — Honolulu, HI
**Generated with the aid of Meta AI**
