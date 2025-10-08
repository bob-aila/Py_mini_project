# Student Registration Number Generator

## 📘 Overview

This project is a simple **Python-based student registration number generator** designed to create unique registration numbers for students.
It automates the generation process by using student details such as name and department code, then saves the generated registration numbers to a file for easy record-keeping.

The project is lightweight, can run locally or online (e.g., on Google Colab or Replit), and can easily be adapted into a web app or command-line interface.

---

## 🎯 Objective

To generate and manage student registration numbers automatically, reducing human error and ensuring a consistent format across records.

---

## ⚙️ Features

* Generates unique registration numbers for each student.
* Saves registration data to a local text file (`students_registry.txt`).
* Allows searching for a student by registration number.
* Modular design with reusable Python functions.
* Can be extended to integrate with databases or web frontends.

---

## 🧩 Algorithm Summary

1. Accept student details (e.g., full name, department).
2. Normalize the name and extract relevant components.
3. Generate a unique registration number using defined rules.
4. Save the record to a file.
5. Allow searching for a record by registration number.

---

## 🧠 Key Python Functions

### 1. `normalize_name(name)`

* **Input:** Raw student name (string)
* **Task:** Cleans and standardizes the name (removes spaces, converts to uppercase).
* **Output:** Normalized name (string)

### 2. `extract_consonants(name)`

* **Input:** Normalized student name
* **Task:** Extracts consonants from the name for use in registration ID
* **Output:** String of consonants

### 3. `generate_reg_number(name, department)`

* **Input:** Student name and department code
* **Task:** Combines parts of name, department, and a random number to create a registration ID
* **Output:** Unique registration number (string)

### 4. `save_student(name, reg_number)`

* **Input:** Student name and registration number
* **Task:** Appends student details to the file `students_registry.txt`
* **Output:** None (writes to file)

### 5. `search_student(reg_number)`

* **Input:** Registration number (string)
* **Task:** Searches the file for a matching record
* **Output:** Matching student details if found, otherwise "Not found"

---

## 💾 File Structure

```
├── registration_numbers.ipynb
├── students_registry.txt
├── README.md
```

---

## 🚀 How to Run

### Option 1: Local Machine

1. Clone this repository:

   ```
   git clone https://github.com/yourusername/student-registration-generator.git
   ```
2. Navigate into the folder:

   ```
   cd student-registration-generator
   ```
3. Run the program:

   ```
   python student_registration.py
   ```

### Option 2: Google Colab

* Open this link: [Colab Notebook](https://colab.research.google.com/github/bob-aila/Py_mini_project/blob/main/registration_numbers.ipynb#scrollTo=4c6114cb)
* Copy-paste the code into a new notebook cell and run.

### Option 3: Replit

* Import the repository directly into Replit using the GitHub link.
* Run the Python script in the Replit IDE.

---

## 🔍 Example Output

```
Enter student name: John Doe
Enter department code: CS
Generated Registration Number: CS-JD-1024
Saved successfully to students_registry.txt
```

Search example:

```
Enter registration number to search: CS-JD-1024
Student found: John Doe (CS-JD-1024)
```

---

## 🧱 Future Improvements

* Add user interface (web or desktop).
* Integrate with an SQL or Firebase database.
* Enable export to Excel or CSV.
* Include input validation and error handling.

---

## 📄 License

This project is released under the MIT License.
You are free to use, modify, and distribute it with proper attribution.
