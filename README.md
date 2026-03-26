# AI-CHATBOT
#CELL-1

Installation of Required Libraries
In this cell, we install the necessary Python libraries required to build the College ERP AI Chatbot system.

Streamlit :
Streamlit is a Python framework used to create web applications easily. In our project, it is used to design the user interface of the ERP chatbot.

Pyngrok :
Google Colab does not allow direct hosting of web applications. So, we use Pyngrok to generate a public URL that allows us to access the Streamlit application through a browser.

Pandas :
Pandas is a data analysis library used to store and manage structured data. In this project, student records such as roll number, marks, attendance, and exam date are stored using Pandas DataFrame.

These libraries are technical foundation of our project.

#CELL-2

Creating the streamlit app
This cell creates the main application file (app.py) which contains the whole chatbot program.

The code displays the title:
AI Chatbot for College ERP

This will appear at the top of the webpage.

Student Data Input

The program creates input boxes for:
Roll Number

Student Name

Attendance

Marks

Exam Date

The user enters student information through these input boxes.

Add Student Button
When the user clicks Add Student:
The system checks whether all fields are filled.

It checks if the roll number already exists.

If the roll number is unique, the student data is stored.

This prevents duplicate roll numbers.

Store Data
The student data is stored in session state and converted into a pandas DataFrame.

A DataFrame is like a table that contains rows and columns.

Display Student Data
If student records exist, the system shows them as a table on the webpage.

This allows the user to see all stored student information.

Chatbot Section
Enter Roll Number

The user enters their roll number so the chatbot can find their details.

Chatbot Logic
The chatbot checks the searches for keywords.

If that contains:
attendance -> The chatbot shows the student's attendance.

marks -> The chatbot shows the student's marks.

exam -> The chatbot shows the exam date.

If they ask differently, the chatbot says it can only answer about attendance, marks, or exam.

Performance Check
The chatbot also checks student performance.

If attendance is below 75%, it tells the student to improve attendance.

If marks are below 35, it tells the student to improve marks.

#CELL-3

Deployment using Ngrok
Google Colab does not allow direct hosting of web servers.

Therefore:
We run the Streamlit application.
Pyngrok creates a secure public URL.
This URL allows external access to the web application.

Purpose:
To simulate deployment of the ERP system.
To make the chatbot accessible via browser.
To demonstrate practical implementation of web hosting.
