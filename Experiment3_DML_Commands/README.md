# Experiment 3: DML Commands

## AIM
To study and implement DML (Data Manipulation Language) commands.

## THEORY

### 1. INSERT INTO
Used to add records into a relation.
These are three type of INSERT INTO queries which are as
A)Inserting a single record
**Syntax (Single Row):**
```sql
INSERT INTO table_name (field_1, field_2, ...) VALUES (value_1, value_2, ...);
```
**Syntax (Multiple Rows):**
```sql
INSERT INTO table_name (field_1, field_2, ...) VALUES
(value_1, value_2, ...),
(value_3, value_4, ...);
```
**Syntax (Insert from another table):**
```sql
INSERT INTO table_name SELECT * FROM other_table WHERE condition;
```
### 2. UPDATE
Used to modify records in a relation.
Syntax:
```sql
UPDATE table_name SET column1 = value1, column2 = value2 WHERE condition;
```
### 3. DELETE
Used to delete records from a relation.
**Syntax (All rows):**
```sql
DELETE FROM table_name;
```
**Syntax (Specific condition):**
```sql
DELETE FROM table_name WHERE condition;
```
### 4. SELECT
Used to retrieve records from a table.
**Syntax:**
```sql
SELECT column1, column2 FROM table_name WHERE condition;
```
**Question 1**
--
-- ![image](https://github.com/user-attachments/assets/9958cd61-4ea8-48d2-bc93-7d42675d5292)


```sql
-- UPDATE products SET reorder_lvl=reorder_lvl*0.7 WHERE product_name LIKE "%cream%" AND quantity>reorder_lvl;
```

**Output:**

![image](https://github.com/user-attachments/assets/609b7094-0f70-4260-acde-53e65bfdccef)


**Question 2**
---
-- ![image](https://github.com/user-attachments/assets/d7eef7a8-d94f-4322-9746-f3c6db6791af)


```sql
-- UPDATE customer SET grade=5 WHERE city="Chennai";
```

**Output:**

![image](https://github.com/user-attachments/assets/7ce7d6e1-c73f-46b4-ad95-d5c375b7e0ae)


**Question 3**
---
-- ![image](https://github.com/user-attachments/assets/9b50723c-b554-4cbe-a5e1-82c80105726d)


```sql
-- UPDATE employees SET email="Unavailable";
```

**Output:**

![image](https://github.com/user-attachments/assets/a62e7c85-0913-46dc-8ea4-9d873b9f3043)


**Question 4**
---
-- ![image](https://github.com/user-attachments/assets/b360c473-1786-47dc-a6fe-6685b7b9bbfd)


```sql
--UPDATE products SET sell_price=sell_price*1.15 WHERE quantity<50 AND supplier_id=10;
```

**Output:**

![image](https://github.com/user-attachments/assets/aa42a198-f13e-472b-952e-59123a4d56c0)


**Question 5**
---
-- ![image](https://github.com/user-attachments/assets/e253473c-7dab-439c-a701-f307801fc665)

```sql
-- UPDATE sales SET total_sell_price=quantity*sell_price WHERE product_id=10;
```

**Output:**

![image](https://github.com/user-attachments/assets/30711432-8730-44f0-9aa0-3a6b2cdd633d)

**Question 6**
---
-- ![image](https://github.com/user-attachments/assets/aaf9581a-52ff-4f8f-ae27-37616af0b20d)


```sql
-- DELETE FROM customer WHERE GRADE>=2;
```

**Output:**

![image](https://github.com/user-attachments/assets/8d8cc402-d338-4a2d-ade6-41cde38f58c8)


**Question 7**
---
-- ![image](https://github.com/user-attachments/assets/2b2c11be-11df-4608-99e2-2dc638037d84)


```sql
-- DELETE FROM customer WHERE cust_country="India" AND cust_city!="Chennai";
```

**Output:**

![image](https://github.com/user-attachments/assets/543bf1b8-628d-4785-a036-bc8cd418d799)


**Question 8**
---
-- ![image](https://github.com/user-attachments/assets/524fdad2-98c7-4564-9c4f-e07753192e7a)

```sql
-- DELETE FROM customer WHERE cust_city!="New York" AND outstanding_amt>5000;
```

**Output:**

![image](https://github.com/user-attachments/assets/60add631-de79-4cd7-9b76-013f557c3ccc)


**Question 9**
---
-- ![image](https://github.com/user-attachments/assets/a62be8f2-1826-4d54-8cef-8c278791c3e9)


```sql
-- DELETE FROM Customer WHERE cust_country="UK" AND working_area="London" AND grade<3;
```

**Output:**

![image](https://github.com/user-attachments/assets/a8a9b1af-e7f6-422d-86c0-e2d9aec2513f)

**Question 10**
---
-- ![image](https://github.com/user-attachments/assets/9954e74b-b9c0-4287-9087-21deaf7bb685)


```sql
-- delete from customer where grade%2!=0;
```

**Output:**

![image](https://github.com/user-attachments/assets/e31f1798-f827-450a-a552-a866d89fb943)


## RESULT
Thus, the SQL queries to implement DML commands have been executed successfully.
