# Genomic CSV Public — Libre 3 Interstitial Glucose Variability

This repository tracks interstitial glucose variability from the business end of the Libre 3 sensor onward.

Think of this repo as a fleet: different boats, same water.

### The Fleet — Three Boats, Three Purposes

**1. Introduction Canoe — `Introduction-To-My-Latest-Relevant-Dataset-10-30-26.pdf` + `Libre-Intro-10-30-26.png`**
- The starting canoe — sensor setup, dataset introduction, and context from Oct 30
- How the Libre 3 data is collected, what Notes mean, and the protocol for tracking
- Read this first if you are new to the dataset

**2. Evaluation Boat #2 — `Evaluation-GBP-Carb-Suppressor-With-Graph.pdf` (V02 perfect final)**
- The evaluation boat — focused fiber evaluation using Sensor #2
- **12-Hour Graph (Nov 1) - 89 mg/dL In Range**
- **Baseline-Matched Overlay — Corrected Legend:**
  - Orange = 5g dextrose only in 8 oz water (iAUC 657.6 mg/dL·min, peak 106)
  - Blue = 5g dextrose + 2.5g GBP in 8 oz water (iAUC 518.7 mg/dL·min, peak 92.5 adj) = **21.1% lower with GBP**
- Method: Peak 1 end baseline 87 mg/dL extrapolated to match Peak 2 end 93 mg/dL (+6.0 mg/dL linear ramp), raw data every 5 min, trapezoidal AUC
- Total AUC: 7,839.5 vs 9,195.5

**3. Evaluation Boat #3 — `Evaluation-GBP-Modifying-Shape-Previous-Peak.pdf` (NEW)**
- **Title:** Modifying the Shape of the Previous Peak
- **Mission Data Complete:**
  - Wave 1 WITH GBP: Peak 161, stone at 85-90, never <70, floor 75
  - Wave 2 WITHOUT GBP: Peak 150, no stone, bottom 69, dips to 70→, recovered to 73
  - **Same meal. Same peak height. Different floor.**
- **Meal:** Salad with large tomato + 1/2 cup sweet potato + two small Jimmy Dean sausage and biscuit + 1 cup watermelon ± 1 tsp GBP
  - Wave 1: Nov 1 21:48 WITH 1 tsp GBP → Peak 161, min 75, stone present
  - Wave 2: Nov 2 06:53 WITHOUT GBP → Peak 150, min 69, no stone
- **Graph:** Overlay both waves aligned at meal start (minutes since meal), green dotted stone zone 85-90, callout box "GBP prevents hypoglycemia without reducing peak" — clean, clinical, no extra variables
- **Bottom confirmed:** Current 70 mg/dL → Glucose In Range, Wave 2 finished 66→73 and leveling

### Data — The Water Both Boats Float On

- **JohnHasty_glucose_11-2-2026.csv** — Single source of truth, superset of all previous data. Libre export through Nov 2 12:16 PM, includes Wave 1 and Wave 2 meals, bottom confirmation, Cocktail notes, and 70 mg/dL Going Low event. All necessary data documented in one CSV file. Older 11-1 CSV removed as duplicate (Option B — history preserved in git).
  - Nov 1: mean 86.1, median 87, min 67, max 106, SD 7.7
  - Acclimation Window (Hour 1-12) n=132 mean 85.5 range 67-106
  - Stable Baseline (Hour 12+) n=39 mean 88.8 range 70-100
  - Protocol: Hour 0-1 Warm-up, Hour 1-12 Acclimation Window, Hour 12+ Stable Baseline — flag don't drop
  - Key Notes: 21:48 PM meal WITH GBP, 06:53 Meal WITHOUT GBP, Cocktail in, 70 mg/dL Going Low

### Repo Purpose

From the business end of the Libre 3 sensor onward, this repo will continue to track interstitial glucose variability — new datasets, new evaluations, same transparent method.

**Author:** John Hasty — Honolulu, HI **Generated with the aid of Meta AI**
