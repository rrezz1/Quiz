# SQL Test Questions — Easy to Mid Level

> 20 multiple-choice questions covering fundamental to intermediate SQL concepts.
> Each question includes the correct answer and an explanation.

---

## Table of Contents

- [Easy Questions (1–10)](#easy-questions-110)
- [Mid-Level Questions (11–20)](#mid-level-questions-1120)
- [Answer Key](#answer-key)

---

## Easy Questions (1–10)

### Q1. What does `SELECT * FROM employees;` return?

- A) All columns from the employees table ✅
- B) Only the first column
- C) Only distinct rows
- D) All tables in the database

> **Explanation:** `SELECT *` retrieves all columns from the specified table.

---

### Q2. Which clause is used to filter rows in a query?

- A) ORDER BY
- B) GROUP BY
- C) WHERE ✅
- D) HAVING

> **Explanation:** `WHERE` filters individual rows before any grouping occurs.

---

### Q3. What is the correct SQL keyword to remove duplicate rows from results?

- A) UNIQUE
- B) DISTINCT ✅
- C) NODUPE
- D) FILTER

> **Explanation:** `SELECT DISTINCT` removes duplicate rows from the result set.

---

### Q4. Which SQL statement is used to insert a new row into a table?

- A) ADD INTO
- B) PUSH INTO
- C) INSERT INTO ✅
- D) CREATE INTO

> **Explanation:** `INSERT INTO table_name VALUES (...)` adds a new row.

---

### Q5. What does NULL mean in SQL?

- A) Zero
- B) Empty string
- C) Unknown / missing value ✅
- D) False

> **Explanation:** `NULL` represents an unknown or missing value — it is not zero or empty string.

---

### Q6. Which aggregate function returns the number of rows?

- A) SUM()
- B) MAX()
- C) COUNT() ✅
- D) AVG()

> **Explanation:** `COUNT()` returns the number of rows matching the query.

---

### Q7. Which clause sorts query results?

- A) SORT BY
- B) ORDER BY ✅
- C) ARRANGE BY
- D) GROUP BY

> **Explanation:** `ORDER BY` sorts results — `ASC` (default) or `DESC`.

---

### Q8. What SQL keyword is used to update existing data?

- A) MODIFY
- B) ALTER
- C) CHANGE
- D) UPDATE ✅

> **Explanation:** `UPDATE table SET col = value WHERE condition;`

---

### Q9. Which command deletes all rows from a table but keeps its structure?

- A) DROP TABLE
- B) DELETE FROM
- C) TRUNCATE TABLE ✅
- D) REMOVE TABLE

> **Explanation:** `TRUNCATE` removes all rows quickly and keeps the table schema intact.

---

### Q10. Which operator checks for a value within a list?

- A) BETWEEN
- B) LIKE
- C) IN ✅
- D) EXISTS

> **Explanation:** `IN (val1, val2, ...)` checks membership in a list of values.

---

## Mid-Level Questions (11–20)

### Q11. What is the difference between WHERE and HAVING?

- A) No difference
- B) WHERE filters before grouping; HAVING filters after grouping ✅
- C) HAVING filters before grouping; WHERE filters after grouping
- D) WHERE only works with JOINs

> **Explanation:** `WHERE` filters rows before `GROUP BY`; `HAVING` filters aggregated groups.

---

### Q12. What will this query return?

```sql
SELECT department, COUNT(*) AS total
FROM employees
GROUP BY department
HAVING COUNT(*) > 5;
```

- A) All departments
- B) Departments with more than 5 employees ✅
- C) Employees with more than 5 records
- D) Nothing — syntax error

> **Explanation:** `GROUP BY` + `HAVING COUNT(*) > 5` returns only departments that have more than 5 employees.

---

### Q13. Which JOIN returns all rows from both tables, filling NULLs where there is no match?

- A) INNER JOIN
- B) LEFT JOIN
- C) RIGHT JOIN
- D) FULL OUTER JOIN ✅

> **Explanation:** `FULL OUTER JOIN` returns all rows from both sides, with NULLs for non-matching rows.

---

### Q14. What does this return if a matching row doesn't exist in table B?

```sql
SELECT a.id, b.name
FROM a LEFT JOIN b ON a.id = b.id;
```

- A) The row is skipped
- B) NULL for b.name ✅
- C) An error
- D) An empty string

> **Explanation:** `LEFT JOIN` keeps all rows from the left table; `b.name` is NULL when no match exists in `b`.

---

### Q15. What is a PRIMARY KEY?

- A) Any indexed column
- B) A column that links two tables
- C) A column (or set) that uniquely identifies each row and cannot be NULL ✅
- D) A column that allows duplicate values

> **Explanation:** A `PRIMARY KEY` must be unique and NOT NULL — it uniquely identifies every row.

---

### Q16. Which of these correctly uses a subquery?

- A) `SELECT * FROM (SELECT id FROM orders) AS sub;` ✅
- B) `SELECT * FROM SELECT id FROM orders;`
- C) `SELECT id FROM * WHERE orders;`
- D) `SELECT SUBQUERY(id) FROM orders;`

> **Explanation:** A subquery in the `FROM` clause must be aliased (e.g. `AS sub`).

---

### Q17. What does `COALESCE(a, b, c)` return?

- A) The sum of a, b, c
- B) The average
- C) The first non-NULL value among a, b, c ✅
- D) Always returns c

> **Explanation:** `COALESCE` returns the first non-NULL value from its list of arguments.

---

### Q18. What is the result of this query?

```sql
SELECT name
FROM products
WHERE price BETWEEN 10 AND 50;
```

- A) Products with price > 10 and < 50
- B) Products with price >= 10 and <= 50 ✅
- C) Products with price = 10 or price = 50
- D) A syntax error

> **Explanation:** `BETWEEN` is inclusive — it includes both boundary values (10 and 50).

---

### Q19. Which window function assigns a unique sequential number to rows within a partition?

- A) COUNT()
- B) RANK()
- C) ROW_NUMBER() ✅
- D) DENSE_RANK()

> **Explanation:** `ROW_NUMBER()` assigns a unique sequential integer with no gaps or ties within the partition.

---

### Q20. What does the FOREIGN KEY constraint enforce?

- A) Unique values in the column
- B) That values exist in a referenced table (referential integrity) ✅
- C) NOT NULL values
- D) Indexed lookups

> **Explanation:** A `FOREIGN KEY` ensures the value exists in the referenced parent table, enforcing referential integrity.

---

## Answer Key

| # | Level | Answer |
|---|-------|--------|
| 1 | Easy | A |
| 2 | Easy | C |
| 3 | Easy | B |
| 4 | Easy | C |
| 5 | Easy | C |
| 6 | Easy | C |
| 7 | Easy | B |
| 8 | Easy | D |
| 9 | Easy | C |
| 10 | Easy | C |
| 11 | Mid | B |
| 12 | Mid | B |
| 13 | Mid | D |
| 14 | Mid | B |
| 15 | Mid | C |
| 16 | Mid | A |
| 17 | Mid | C |
| 18 | Mid | B |
| 19 | Mid | C |
| 20 | Mid | B |

---

*Generated for SQL knowledge assessment — Easy to Mid level.*
