# Abstract — Draft v2.0

**Paper Title:**
Evaluation Methodology and Data Resolution Jointly 
Determine Whether Temporal Architectures Outperform 
Feedforward Models in Environmental Prediction

**Key Contributions:**

1. Temporal leakage inflates LSTM advantage by 3× 
   under non-causal random splits

2. Sequence length sweep reveals inverted-U temporal 
   regime peaking at 60 minutes — corresponding to 
   physical irrigation event duration

3. Downsampling induces a phase transition where 
   temporal models lose their advantage due to loss 
   of physically meaningful temporal structure — 
   LSTM advantage inverts from +23% to -120% as 
   sampling rate decreases from 1-minute to 10-minute 
   resolution

**Killer sentence:**
"Under random splits, LSTM performance improvements 
increase from ~6% to ~17%, suggesting that commonly 
used evaluation strategies substantially overestimate 
the benefits of temporal modeling."

**Reviewer defense — two known weaknesses:**

1. Small sample bias at 360-minute rate (133 samples)
   Defense: "Performance degradation is partially 
   attributable to reduced sample size, but the trend 
   is consistent across intermediate regimes"

2. LSTM collapse might look like poor tuning
   Defense: Same architecture across all regimes — 
   controlled comparison eliminates tuning as 
   confounding variable

**Updated paper title:**
"Evaluation Methodology and Data Resolution Jointly 
Determine Whether Temporal Architectures Outperform 
Feedforward Models in Environmental Prediction: 
Evidence from Physics-Aware Soil Moisture Sensing"

**Target:** IEEE Geoscience and Remote Sensing Letters
**Status:** Draft v2.0 — Issues #5 + #6 complete
