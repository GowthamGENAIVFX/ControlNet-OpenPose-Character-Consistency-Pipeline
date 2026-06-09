# Optimization Notes

## Objective

Improve pose consistency while maintaining image quality.

---

# Experiment 1

## ControlNet Weight

### Test Values

0.5

0.7

1.0

1.2

### Result

0.8 to 1.0 produced the most reliable pose matching.

---

# Experiment 2

## CFG Scale

### Test Values

5

7

9

### Result

CFG 7 provided the best balance.

---

# Experiment 3

## Sampling Steps

10

20

30

50

### Result

30 steps delivered the best quality-to-performance ratio.

---

# Experiment 4

## LoRA Strength

0.4

0.8

1.2

### Result

0.8 produced consistent stylistic enhancement without artifacts.

---

# Key Learnings

* ControlNet is highly dependent on pose quality.
* OpenPose works best with clear human figures.
* Excessive CFG values reduce natural image variation.
* High ControlNet weights can over-constrain outputs.

---

# Production Recommendations

Control Weight: 0.8

Steps: 30

CFG: 7

LoRA Strength: 0.8

Resolution: 1024x1024
