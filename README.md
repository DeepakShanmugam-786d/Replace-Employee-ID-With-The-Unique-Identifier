# 🏢 Replace Employee ID with Unique Identifier

## 📌 Problem Description

We have two tables:

### **1️⃣ Employees Table** (Stores employee details)
| Column Name | Type    |
|------------|--------|
| id         | int    |
| name       | varchar |

- **id**: A unique number assigned to each employee.
- **name**: The name of the employee.

### **2️⃣ EmployeeUNI Table** (Stores unique IDs for some employees)
| Column Name | Type    |
|------------|--------|
| id         | int    |
| unique_id  | int    |

- **id**: Employee ID (matches the Employees table).
- **unique_id**: A special ID assigned to some employees.

---

## 🎯 Goal: Match Employee IDs with Unique IDs
We need to **find the unique_id for each employee**. If an employee **does not** have a unique_id, we should show **NULL**.

### ✅ Expected Output
| unique_id | name     |
|-----------|---------|
| null      | Alice    |
| null      | Bob      |
| 2         | Meir     |
| 3         | Winston  |
| 1         | Jonathan |

### 🔍 Explanation:
- **Alice and Bob** do not have a unique ID → **NULL**
- **Meir’s unique ID is 2**
- **Winston’s unique ID is 3**
- **Jonathan’s unique ID is 1**

---

## 🔥 How to Solve
1️⃣ **Join the Employees table with the EmployeeUNI table** using the **id** column.  
2️⃣ **If an employee doesn’t have a unique_id, return NULL.**  
3️⃣ **Return the unique_id and the employee’s name.**

---

## 🏆 Why is this important?
- **Helps in proper employee identification** 🆔
- **Ensures data consistency in company records** 📊
- **Practical example of SQL Joins & Null Handling** 🔍

🚀 Now you’re ready to write a query and solve this problem efficiently!

