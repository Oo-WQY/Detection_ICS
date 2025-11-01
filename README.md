# Detection_ICS Dataset

The **Detection_ICS** dataset contains two subsets designed for automated immunochromatographic test strip (ICS) analysis:

1. **Classification Dataset**  
2. **Quantitative Regression Dataset**

**Directory structure:**
```text
Detection_ICS
└── datasets2class
    ├── 0-notarget
    ├── 1-poorquality
    ├── 2-invalidstrip
    ├── 3-negative
    └── 4-positive
└── datasets2quantiy
    ├── 5-(mlU/ml)
    ├── 10-(mlU/ml)
    ├── 25-(mlU/ml)
    ├── 50-(mlU/ml)
    ├── 175-(mlU/ml)
    ├── 100-(mlU/ml)
    ├── 200-(mlU/ml)
    └── 300-(mlU/ml)
```

---

## 1. Classification Dataset

This subset is intended for **test strip result classification** tasks.  
It contains **five classes**, each representing a different test strip condition:

| Class ID | Class Name     | Description                                  |
|-----------|----------------|----------------------------------------------|
| 0 | **notarget** | No test strip present |
| 1 | **poorquality** | Poor image quality |
| 2 | **invalidstrip** | Invalid test strip (e.g., control line failure) |
| 3 | **negative** | Negative result (0 mlU/ml) |
| 4 | **positive** | Positive result (test line detected) |


Each folder contains image samples belonging to the corresponding category.

---

## 2. Quantitative Regression Dataset

This subset is designed for **quantitative concentration estimation** of ICS results.  
It includes **nine folders**, where each folder name corresponds to a **concentration level (mlU/ml)**:

| Folder Name | Concentration (mlU/ml) |
|--------------|------------------------|
| 5 | 5 |
| 10 | 10 |
| 25 | 25 |
| 50 | 50 |
| 75 | 75 |
| 100 | 100 |
| 150 | 150 |
| 200 | 200 |
| 300 | 300 |



Each folder contains test strip images collected at the specified concentration level.

---

## 3. Citation and Author

**Author:** Qingyue Wang  
**Date:** October 31, 2025  
**Dataset Name:** Detection_ICS