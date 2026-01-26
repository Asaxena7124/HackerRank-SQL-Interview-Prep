# 🧩 Revising the Select Query I – HackerRank

## 📝 Problem Statement
![Question](question.png)

---

## ✅ Solution (Visual)
![Solution](solution.png)

---

## 🧾 SQL Solution (Copy-Friendly)

```sql
SELECT *
FROM CITY
WHERE POPULATION > 100000
  AND COUNTRYCODE = 'USA';
```

## 🧠 SQL Clauses Used & Explanation

### 🔹 SELECT
Used to specify which columns to retrieve from the table.

**Why used here:**  
`SELECT *` is used because the problem explicitly requires all columns.

**Interview angle:**  
Interviewers often ask when `SELECT *` should be avoided.

**Common mistake:**  
Using `SELECT *` in production queries instead of selecting only required columns.

---

### 🔹 FROM
Specifies the table from which data is fetched.

**Why used here:**  
The required data is stored in the `CITY` table.

**Interview angle:**  
Tests basic understanding of SQL query structure.

---

### 🔹 WHERE
Filters rows based on specified conditions.

**Why used here:**  
Filters cities with population greater than 100000 and belonging to the USA.

**Interview angle:**  
Very common topic to test filtering logic and SQL execution order.

**Common mistake:**  
Using `WHERE` with aggregate functions instead of `HAVING`.

---

### 🔹 AND
Combines multiple conditions in the `WHERE` clause.

**Why used here:**  
Ensures both population and country conditions must be satisfied.

**Interview angle:**  
Tests understanding of logical operators.

**Common mistake:**  
Confusing `AND` with `OR`, leading to incorrect result sets.

---

## 🎯 Interview Questions & How to Answer

### Q1. What is the difference between `WHERE` and `HAVING`?
**Answer:**  
`WHERE` filters individual rows before aggregation, whereas `HAVING` filters grouped results after aggregation.

---

### Q2. Why should `SELECT *` be avoided in production queries?
**Answer:**  
It retrieves unnecessary columns, increases I/O cost, and can negatively impact query performance.

---

### Q3. Does the order of conditions in the `WHERE` clause matter?
**Answer:**  
Logically no. SQL query optimizers may reorder conditions internally for better performance.

---

### Q4. What would happen if `OR` was used instead of `AND` in this query?
**Answer:**  
The query would return cities that either have population greater than 100000 **or** belong to the USA, resulting in a larger and incorrect dataset.

---

### Q5. In what order does SQL execute this query?
**Answer:**  
1. `FROM`  
2. `WHERE`  
3. `SELECT`

---

## 📌 Key Takeaways
- Always filter data early using the `WHERE` clause
- Clearly understand logical operators (`AND`, `OR`)
- Write readable queries for better interview communication
- Knowing execution order helps in optimization discussions
