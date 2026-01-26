# 🧩 Revising the Select Query I – HackerRank

## 📝 Problem Statement
![Question](question.png)

---

## ✅ Solution
![Solution](solution.png)

---

## 🧠 SQL Clauses Used & Explanation

### 🔹 SELECT
Used to choose the columns from the table.
- `SELECT *` retrieves all columns
- In interviews, avoid `SELECT *` unless explicitly required

### 🔹 FROM
Specifies the source table (`CITY`).

### 🔹 WHERE
Filters rows based on conditions.
- Executed before `SELECT`
- Common interview topic

### 🔹 AND
Combines multiple filtering conditions.
- All conditions must be true

---

## 🎯 Interview Questions & How to Answer

### Q1. What is the difference between `WHERE` and `HAVING`?
**Answer:**  
`WHERE` filters rows before aggregation, while `HAVING` filters groups after aggregation.

### Q2. Why should `SELECT *` be avoided in production?
**Answer:**  
It retrieves unnecessary columns, increases I/O cost, and affects performance.

### Q3. Does the order of conditions in `WHERE` matter?
**Answer:**  
Logically no, but query optimizers may reorder them for performance.

---

## 📌 Key Takeaways
- Filtering reduces dataset size early
- Always write readable and optimized queries
- Understand clause execution order for interviews

---

## 🔗 References
- HackerRank SQL Practice
