# etch-depth-dmaic-optimization
Optimized semiconductor etch process using DMAIC, achieving 72% reduction in variability through SPC and statistical testing.
## 🎯 Objective

- Minimize variability in etch depth across wafers
- Improve process control and shift the mean toward 930 nm
- Identify and optimize critical process parameters

---

## 🔍 Methodology: DMAIC Framework

### 1. Define

- **Problem**: Excessive etch depth variation causing downstream defects and yield loss
- **Goal**: Reduce etch variability by ≥ 60% and align output within ±5% spec limits

---

### 2. Measure

Data was collected across 60 wafers, split into **Before** and **After** optimization groups. Each wafer was evaluated for:
- Etch Depth (nm)
- RF Power (W)
- Chamber Pressure (mTorr)
- Gas Flow (sccm)
- Etch Time (s)

#### 📷 Control Chart – Combined View
![Control Chart]("C:\Users\shlok\Desktop\Projects\Improved_Etch_Process_Data__60_Rows_ - Control Chart Builder of Etch Depth (nm).png")

This X̄ & R control chart illustrates the overall trend in process stability. The lower half (Range chart) clearly shows a shift at subgroup 7 — after process optimization — where variability drops significantly.

---

### 3. Analyze

#### 📷 Control Charts – Before vs. After
![Control Chart - Before and After]("C:\Users\shlok\Desktop\Projects\Improved_Etch_Process_Data__60_Rows_ - Control Chart Builder.png")

- **Before Optimization**: Wide range with UCL at ~74, indicating large spread.
- **After Optimization**: Range drops to ~21, showing a **72% reduction** in process spread.

#### 📷 Distribution Plots
![Distributions - Before and After]("C:\Users\shlok\Desktop\Projects\Improved_Etch_Process_Data__60_Rows_ - Distribution.png")

- The “Before” distribution is wider and skewed right.
- The “After” distribution is tighter with a lower mean — a clear shift toward the target of 930 nm.

#### 📷 t-Test and Variance Analysis
![t-Test and Variance Analysis]("C:\Users\shlok\Desktop\Projects\Improved_Etch_Process_Data__60_Rows_ - Fit Y by X of Etch Depth (nm) by Condition.png")

- Welch’s t-test shows p < 0.0001, confirming a statistically significant shift in mean.
- Levene’s and Bartlett’s tests confirm the variance reduction is significant.
- Standard deviation dropped from **13.56 nm** to **4.50 nm**.

---

### 4. Improve

#### 📷 Multivariate Correlation and Regression
![Multivariate Correlation]("C:\Users\shlok\Desktop\Projects\Improved_Etch_Process_Data__60_Rows_ - Multivariate.png")

- **RF Power** has a strong positive correlation with etch depth (r = +0.43).
- **Chamber Pressure** shows a moderate inverse relationship (r = –0.30).
- Based on this, RF Power and Chamber Pressure were optimized to operate within tighter, more stable ranges.

---

### 5. Control

- SPC charts were implemented for ongoing weekly review.
- SOPs were updated, and operators were trained on new parameter ranges.
- Any two consecutive points outside ±3σ will trigger root cause analysis.

---

## 📈 Results Summary

| Metric               | Before       | After        | % Change         |
|----------------------|--------------|--------------|------------------|
| Mean Etch Depth (nm) | 931.99       | 921.05       | ↓ 10.94 nm       |
| Std Dev (nm)         | 13.56        | 4.50         | ↓ 66.8%          |
| Range (R̄)           | 34.99        | 10.08        | ↓ **71.2%**      |
| Welch’s Test p-value | —            | < 0.0001     | Statistically significant |

---

## 🛠 Tools Used

- JMP Pro (Statistical analysis)
- Control Charts (X̄ & R)
- Regression & Correlation
- Welch’s t-Test and Levene’s Test
- DMAIC Methodology

---

## ✅ Outcome

- Reduced etch depth variability by 71%, improving wafer quality and yield.
- Achieved stable process performance through parameter control.
- Enabled long-term monitoring with SPC and statistical alerts.

---
