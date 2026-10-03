# 🩺 Python Medical Records Validator

A robust Python script designed to validate structured medical records and patient datasets. It ensures data integrity by checking key consistency, data types, value constraints, and regular expression patterns (e.g., patient IDs and visit IDs).

---

## 🚀 Features

*   **Structure Validation:** Ensures the input data is provided as a valid sequence (list/tuple) of dictionaries with exact key matching.
*   **Regex Pattern Matching:** Validates alphanumeric ID formats like `patient_id` (`p\d+`) and `last_visit_id` (`v\d+`) case-insensitively using Python's `re` module.
*   **Type & Constraint Checking:** Verifies age ranges (e.g., adults $\ge 18$), accepted gender categories, and medication list items.
*   **Detailed Error Logging:** Pinpoints exact dictionary positions and keys that violate validation rules.

---

## 📂 Project Structure

```text
├── validator.py      # Contains validation functions and sample medical records
└── README.md         # Project documentation
from validator import validate, medical_records

# Validate the records
is_valid = validate(medical_records)
