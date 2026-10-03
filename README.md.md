# ML Assignment 1 — NumPy: Vectorised Computation

**Repository Name**: `ml-assignment-1-numpy`  
**Submission Task**: Task 1 (Machine Learning Assignments 1 to 4\)

---

## Question 8: Execution Speedup Benchmark

- **Task**: Counting occurrences of each value across 1,000,000 random integers between 0 and 99\.  
- **NumPy (`np.bincount`) Execution Time**: \~1.2 ms  
- **Python Loop Execution Time**: \~45.0 ms  
- **Reported Speedup**: **\~37.5x faster** using vectorized `np.bincount` compared to a plain Python iteration loop.

---

## Repository Contents

- `assignment1_numpy.ipynb`: Complete vectorized computation solutions with zero element-wise Python loops over array elements, including:  
  1. Normal distribution array generation, shape, dtype, and float32 conversion.  
  2. Column-wise standardization via broadcasting.  
  3. Custom arbitrary-axis `minmax` scaling function.  
  4. Random NaN injection (5%) and `np.nanmean` imputation.  
  5. 3-sigma outlier detection and median replacement.  
  6. 200x200 Euclidean distance matrix via broadcasting.  
  7. Top 5 nearest neighbors via `np.argpartition` (\$O(N)\$ linear complexity).  
  8. `%%time` performance comparison.  
  9. Stride tricks `sliding_window_view` matching `pandas.Series.rolling.mean`.  
  10. Array reshaping (12, 8\) \-\> (4, 3, 8\) and chunk averaging.  
  11. `clean.npy` serialization and verification.  
- `README.md`: Benchmark documentation.