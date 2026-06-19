### 📊 Data Analytics & Visual Report

#### Dataset Focus: Davao Region Agricultural Production Index (Mock CSV Analysis)

#### 1. Data Cleaning Protocol Log
* **Raw Input Problem:** The source CSV file (`Davao_Agri_Yield_Q1Q4_Raw.csv`) suffered from severe structural anomalies: missing row data for the critical 2023 climate transition fiscal year, non-standardized units (mixing metric tons, kilograms, and localized market weight counts like *kaing* boxes), and duplicated entries caused by conflicting municipal cooperative codes.
* **AI Cleaning Instruction:** 
```text
  "Scan the attached dataset. Isolate all null values in the 'Yield_Volume' column and impute them using the median value calculated strictly for that specific crop tier and municipality. Standardize all mass metrics to metric tons (MT), stripping out text strings like 'kg' or 'tons'. Consolidate duplicate municipal entries by computing a weighted average across overlapping timestamps. Output the first 5 rows of the cleaned table."
