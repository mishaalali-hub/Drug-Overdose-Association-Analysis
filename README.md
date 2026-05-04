# Drug-Overdose-Association-Analysis

A Data Mining and Association Rule Mining project focused on identifying hidden drug co-occurrence patterns in accidental drug-related death cases using Apriori and FP-Growth algorithms.

This project was developed as part of an individual Data Mining assignment using real-world overdose mortality data.

---

# Project Overview

The purpose of this project is to analyze accidental drug-related death records and discover meaningful relationships between substances involved in overdose incidents.

The project applies:

- Data preprocessing techniques
- Transaction-based data transformation
- Association Rule Mining
- Frequent Itemset Mining
- Pattern Discovery Analysis
- Comparative algorithm evaluation

The analysis focuses on identifying:

- Common drug combinations
- Poly-drug exposure patterns
- Frequent co-occurring substances
- Strong association rules between drugs

---

# Dataset

Dataset Used:
- Accidental Drug Related Deaths Dataset

Source:
- Connecticut Open Data Portal

Dataset File:
- `Accidental_Drug_Related_Deaths_CLEANED_V2.csv`

Dataset Characteristics:
- More than 11,000 overdose records
- Demographic attributes
- Location attributes
- Drug substance indicators
- Transaction-based analytical structure

---

# Technologies Used

## Programming Language
- Python

## Libraries & Frameworks
- Pandas
- NumPy
- Matplotlib
- Seaborn
- mlxtend
- Scikit-learn
- Jupyter Notebook

---

# Project Structure

```bash
Drug-Overdose-Association-Analysis/
│
├── Preprocessing_Code.ipynb
├── Drug-Overdose-Association-Analysis.ipynb
├── README.md
```

---

# Features Implemented

## 1. Data Preprocessing

The preprocessing workflow includes:

- Attribute standardization
- Missing value handling
- Duplicate detection
- Binary transformation of substance indicators
- Data cleaning and validation
- Mining-ready dataset construction

---

## 2. Transaction-Based Data Representation

The dataset was transformed into a transaction matrix where:

- Each overdose case represents a transaction
- Each drug substance represents an item
- Binary encoding was used:
  - 1 = Drug Present
  - 0 = Drug Absent

This structure enables Association Rule Mining algorithms to discover hidden patterns.

---

## 3. Frequency Analysis

Implemented analyses include:

- Substance prevalence analysis
- Drug frequency ranking
- Poly-substance exposure analysis
- Case-level substance count analysis

---

## 4. Co-Occurrence Analysis

The project performs:

- Pairwise substance co-occurrence analysis
- Heatmap visualization
- Most frequent drug pair identification
- Interaction pattern discovery

---

## 5. Association Rule Mining

Implemented algorithms:

- Apriori Algorithm
- FP-Growth Algorithm

Generated outputs include:

- Frequent itemsets
- Association rules
- Support values
- Confidence values
- Lift metrics

---

# Algorithms Used

## 1. Apriori Algorithm

### Why It Was Used

The Apriori algorithm was selected because:

- It is one of the most important association rule mining algorithms
- It identifies frequent itemsets effectively
- It generates interpretable association rules
- It is suitable for transaction-based datasets

### How It Works

Apriori works by:

1. Scanning the transaction dataset
2. Generating candidate itemsets
3. Calculating support values
4. Removing infrequent itemsets
5. Producing association rules from frequent patterns

### Purpose in This Project

The algorithm was used to:

- Discover common drug combinations
- Identify recurring overdose patterns
- Generate meaningful association rules
- Analyze poly-drug relationships

---

## 2. FP-Growth Algorithm

### Why It Was Used

FP-Growth was implemented because:

- It is more computationally efficient than Apriori
- It avoids excessive candidate generation
- It performs well on large datasets
- It uses compressed tree structures

### How It Works

FP-Growth works by:

1. Constructing an FP-Tree
2. Compressing transaction data
3. Mining frequent patterns recursively
4. Extracting association rules efficiently

### Purpose in This Project

FP-Growth helped to:

- Identify frequent drug combinations faster
- Compare mining efficiency against Apriori
- Validate discovered patterns
- Improve scalability for larger datasets

---

## 3. Association Rule Mining

### Why It Was Used

Association Rule Mining was applied to:

- Discover hidden relationships between drugs
- Identify systematic overdose patterns
- Analyze substance interaction trends
- Detect meaningful co-occurrence relationships

### Metrics Used

| Metric | Purpose |
|---|---|
| Support | Measures how often a drug combination occurs |
| Confidence | Measures the probability of relationships between drugs |
| Lift | Measures the strength of association between substances |

---

## 4. Binary Transaction Matrix

### Why It Was Used

Binary transaction transformation was necessary because:

- Association rule algorithms require transactional data
- It standardizes substance representation
- It enables pattern discovery analysis
- It simplifies co-occurrence computations

### How It Works

Each substance indicator was converted into:

- 1 → Substance Present
- 0 → Substance Absent

---

# Included Notebooks

## 1. Preprocessing_Code.ipynb

This notebook focuses on:

- Data cleaning
- Missing value handling
- Binary transformation
- Transaction dataset creation
- Data validation
- Mining-ready dataset preparation

---

## 2. Drug-Overdose-Association-Analysis.ipynb

This notebook focuses on:

- Apriori Algorithm implementation
- FP-Growth Algorithm implementation
- Association Rule Mining
- Frequent itemset generation
- Support, confidence, and lift calculations
- Pattern discovery and visualization

---

# Machine Learning & Mining Workflow

```text
Raw Dataset
    ↓
Data Cleaning & Preprocessing
    ↓
Drug Variable Extraction
    ↓
Binary Transaction Matrix Creation
    ↓
Association Rule Mining
    ↓
Apriori & FP-Growth Analysis
    ↓
Frequent Itemset Discovery
    ↓
Association Rule Generation
    ↓
Pattern Interpretation & Insights
```

---

# How to Run the Project

## 1. Clone the Repository

```bash
git clone https://github.com/yourusername/Drug-Overdose-Association-Analysis.git
cd Drug-Overdose-Association-Analysis
```

---

## 2. Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn mlxtend scikit-learn
```

---

## 3. Open Jupyter Notebook

```bash
jupyter notebook
```

---

## 4. Run the Notebooks

Execute:

- `Preprocessing_Code.ipynb`
- `Drug-Overdose-Association-Analysis.ipynb`

---

# Key Findings

The analysis discovered:

- Strong co-occurrence patterns between opioids and secondary substances
- Frequent combinations involving fentanyl, heroin, cocaine, ethanol, and benzodiazepines
- High prevalence of poly-drug overdose cases
- Meaningful association rules with strong lift values
- Consistent results between Apriori and FP-Growth algorithms

---

# Results

The project successfully:

- Converted raw overdose data into transaction-based format
- Applied Association Rule Mining techniques
- Identified frequent drug combinations
- Generated meaningful association rules
- Compared Apriori and FP-Growth performance
- Visualized substance interaction patterns
- Demonstrated practical applications of Data Mining in healthcare analytics

---

# Academic Purpose

This repository was developed for:

- Educational purposes
- Academic research and learning
- Data Mining coursework demonstration
- Association Rule Mining implementation practice

---

# Future Improvements

Potential future enhancements include:

- Interactive dashboard development
- Real-time overdose trend analysis
- Predictive overdose risk modelling
- Advanced visualization systems
- Deep learning integration
- Explainable AI techniques
- Automated association rule optimization

---

# License

This project is intended for academic and educational purposes only.
