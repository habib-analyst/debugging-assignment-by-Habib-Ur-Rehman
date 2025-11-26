# Debugging Assignment – Admission Task
**Author:** Habib Ur Rehman  
**GitHub:** https://github.com/habib-analyst  

This repository contains my completed solutions for the debugging assignment required for admission.  
Each exercise involved identifying bugs, correcting the logic, and ensuring the updated functions run properly with correct outputs.

---

## 📌 Overview of Debugging Tasks

The notebook includes four exercises.  
Below is a summary of what I fixed in each one.

---

## 🟦 **Exercise 1 – Fixing `id_to_fruit` Indexing Bug**
**Issue Identified:**  
- The original function used a `set`, which is an *unordered* data structure and cannot be indexed safely.

**Fix Implemented:**  
- Replaced the set with a `Sequence[str]` (e.g., list).  
- Added index validation.  
- Returned predictable, correct results based on position.

**Skills Demonstrated:**  
Data structures, type correctness, defensive programming.

---

## 🟩 **Exercise 2 – Fixing In-Place Swap Corruption**
**Issue Identified:**  
- The original coordinate swap overwrote values incorrectly, leading to corrupted bounding boxes.

**Fix Implemented:**  
- Performed the swap using a **safe copy** of the array.  
- Corrected mapping of x/y coordinates for both points.  
- Preserved the class label.

**Skills Demonstrated:**  
NumPy operations, array safety, geometric transformations.

---

## 🟧 **Exercise 3 – Fixing CSV Parsing + Plot Logic**
**Issues Identified:**  
- CSV values were treated as strings.  
- Precision and recall were mixed up in the plot.  
- Axis labels were incorrect.

**Fix Implemented:**  
- Converted CSV values to `float`.  
- Corrected the precision-recall mapping.  
- Updated axis labels and plot formatting.

**Skills Demonstrated:**  
File I/O, CSV parsing, data visualization, debugging silent logic errors.

---

## 🟥 **Exercise 4 – Fixing GAN Training Loop**
**Issues Identified:**  
1. **Structural Bug:**  
   - Label tensors used a fixed batch size instead of the current batch size.  
2. **Cosmetic Bug:**  
   - Generated images displayed only at a specific batch index.  

**Fix Implemented:**  
- Dynamically computed `current_batch_size` for labels and noise.  
- Improved training loop structure.  
- Displayed generated samples at the end of each epoch.

**Skills Demonstrated:**  
Deep learning (PyTorch), GAN architecture understanding, training loop debugging, visualization.

---

## ▶️ **How to Run**
Open the notebook: debugging_assignment_by_Habib_Ur_Rehman.ipynb


Run each cell in order.  
A GPU runtime (Colab or local) is recommended for Exercise 4.

---

## ✔️ Final Notes
This assignment demonstrates my ability to:
- Analyze faulty code  
- Understand expected behavior  
- Apply correct fixes  
- Test and validate results  
- Work across NumPy, CSV, plotting, and PyTorch GANs  

Please feel free to review the notebook directly in this repository.

---

**Thank you for reviewing my submission.**

