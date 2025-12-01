# 📚 Capstone Student Management System (Java)

A fully functional **console-based Student Management System** built in Java using:

* **OOP concepts** (Inheritance, Abstraction)
* **Interfaces**
* **Custom Exception Handling**
* **File Handling (Persistent Storage)**
* **Collections API (Map, List, Iterator)**
* **Multithreading (Loader animation)**

This system provides complete CRUD operations, sorting, searching, persistent saving, and loading of student records.

---

## ✨ Features

### ✅ Add Student

* Automatically calculates grade based on marks
* Validates roll number & marks
* Shows loading animation using multithreading

### ✅ View All Students

* Displays all records stored in memory

### ✅ Search Student

* Searches by **name** (case-insensitive)
* Throws custom `StudentNotFoundException` if not found

### ✅ Delete Student

* Deletes student using roll number
* Updates both map & list

### ✅ Update Student

* Update email, course, and marks
* Recalculates grade automatically

### ✅ Sort by Marks

* Uses `Comparator` for descending order

### ✅ File Handling (students.txt)

* **Auto-loads records** on startup
* **Saves all records** before exiting
* Stores as:

```
rollNo,name,email,course,marks
```

### ✅ Multithreading

A `Loader` class shows animated dots (“Saving...”) whenever writing to file.

---

## 🧠 System Architecture

### **Classes Used**

| Class                      | Description                                      |
| -------------------------- | ------------------------------------------------ |
| `Person`                   | Abstract superclass for common fields            |
| `Student`                  | Child class storing rollNo, course, marks, grade |
| `RecordActions`            | Interface for CRUD operations                    |
| `StudentManager`           | Implements CRUD, file I/O, sorting, searching    |
| `Loader`                   | Runnable for loading animation                   |
| `StudentNotFoundException` | Custom exception                                 |
| `Assignment5_Capstone`     | Main driver class                                |

---

## 📂 File Structure

```
Assignment5_Capstone.java
students.txt
README.md
```

---

## ▶️ How to Run

1. Save the code into **Assignment5_Capstone.java**
2. Compile:

```
javac Assignment5_Capstone.java
```

3. Run:

```
java Assignment5_Capstone
```

---

## 🧪 Sample Menu Output

```
===== Capstone Student Menu =====
1. Add Student
2. View All Students
3. Search Student
4. Delete Student
5. Update Student
6. Sort by Marks
7. Save & Exit
Enter choice:
```

---

## 📝 Error Handling

* Invalid marks → Throws exception
* Duplicate roll number → Throws exception
* Search not found → Custom `StudentNotFoundException`
* Invalid menu input → Gracefully handled

---

## 💡 Why This Project Is Good for Capstone / College

* Implements all major OOP concepts
* Uses exception handling & custom exceptions
* Demonstrates file I/O for persistent storage
* Uses multithreading
* Uses Java Collections extensively
* Menu-driven and user-friendly

---
