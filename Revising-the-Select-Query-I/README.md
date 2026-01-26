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
