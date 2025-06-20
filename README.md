# 📊 NPS Data Processing & SOLID Principles in Python

This project demonstrates how to process Net Promoter Score (NPS) data efficiently using Python while applying **clean coding principles** and **SOLID object-oriented design principles**.

It transforms repetitive data analysis tasks into reusable, testable, and scalable modules using real-world inspired NPS datasets.

---

## 🚀 Features

- 📂 Load and validate multiple NPS CSV files using context managers.
- 🧱 Clean, modular code with function abstraction (DRY principle).
- 🎯 Classify ratings into **Promoters**, **Passives**, and **Detractors**.
- 📈 Calculate NPS globally and by source (email, web, mobile).
- ✅ Full implementation of **SOLID principles**.

---

## 🔧 How It Works

1. **Data Sources**  
   Load NPS responses from multiple CSVs using custom loader classes (`CsvNpsDataSource`).

2. **Rating Categorization**  
   Convert raw ratings into standard categories using interface-based composition.

3. **Validation & Cleaning**  
   Validate structure and ensure data is ready for analysis (`clean_nps_data()`).

4. **Combination & Scoring**  
   Combine datasets and compute NPS using formulas and group-by aggregation.

---

## 🧠 SOLID Principles Applied

| Principle | Implementation |
|----------|----------------|
| **S**ingle Responsibility | Each function/class has one purpose (e.g., loading, cleaning, categorizing) |
| **O**pen/Closed | New sources and categorizers can be added without changing core logic |
| **L**iskov Substitution | Abstract base classes (`NpsDataSource`) ensure interchangeable sources |
| **I**nterface Segregation | Split interfaces for rating logic and validation |
| **D**ependency Inversion | Inject categorizer and validator via constructor for flexibility |

---



---

## 📊 Example Output

```python
email     18.59
web       22.09
mobile   -14.71
dtype: float64
```

---

## 📘 Documentation

- `NPSData.combine_nps_data()` – merges multiple source files
- `calculate_nps()` – calculates NPS from categorized scores
- `calculate_nps_by_source()` – groups and calculates per source

---

## ✍️ Author

This project was built as an educational deep dive into combining **real-world data analysis** with **robust software design**.

> Built with ❤️ by [Your Name Here]

---

## 📜 License

MIT License
