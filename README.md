# college-Dbms-lab-5
# README

## Experiment: JOIN Queries in SQL

### Aim:
To perform data retrieval from multiple related tables using INNER JOIN and understand relationships between entities.

### Description:
Is lab me humne different tables (Student, Enrollment, Course, Faculty, Department) ko JOIN karke combined data nikala. Ye queries relational database ke concept ko practically samjhati hain.

### Requirements:
- Tables properly created hone chahiye
- Primary Key aur Foreign Key relationships defined hone chahiye
- Sufficient data inserted hona chahiye meaningful output ke liye

### Concepts Covered:
- INNER JOIN
- JOIN Condition (PK–FK relation)
- Table Aliases
- Multiple Table JOIN
- Filtering (WHERE clause)
- Sorting (ORDER BY)

### Execution Summary:

- Student aur Enrollment ko join karke student-course relation nikala
- Course aur Faculty ko join karke teaching details retrieve ki
- Teen tables (Student + Enrollment + Course) join karke full academic data nikala
- Department based queries execute ki
- Filtering (DepartmentID) aur Sorting (ascending order) apply ki

### Learning Outcome:
- Multiple tables se data efficiently retrieve karna seekha
- JOIN operations ka real-life use samjha
- Complex queries likhne ki understanding improve hui

### Conclusion:
JOIN queries relational databases ka important part hain. Inka use karke hum easily multiple tables se meaningful information nikaal sakte hain bina data duplicate kiye.

### Sample Query:
SELECT S.Name, E.Semester, C.CourseName
FROM Student S
INNER JOIN Enrollment E ON S.StudentID = E.StudentID
INNER JOIN Course C ON E.CourseID = C.CourseID;
