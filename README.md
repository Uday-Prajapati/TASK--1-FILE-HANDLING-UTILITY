# Name: Prajapati Uday Mukesh
# Company: CODTECH IT SOLUTIONS 
# Id: CT6WDS2794
# Domain: Java Programming
# Duration: DECEMBER 12th, 2024 to JANUARY 27th, 2025.
# Mentor: Muzammil Ahmed

# Overview:
This Java program, FileOperation, provides a comprehensive demonstration of working with text files in Java. It implements three key functionalities: writing content to a file, reading content from a file, and modifying content in a file. The program emphasizes user interaction by allowing the user to input file names, content, and modification details via the console.

# Key Activities:
# 1. Writing to a File:
The program uses a BufferedWriter with a FileWriter to write user-provided content to the specified file.

# 2. Reading from a File:
The program employs a BufferedReader with a FileReader to read the content of the file line by line.

# 3. Modifying a File:
The program reads all lines of the file into a List using the Files.readAllLines() method from the java.nio.file package.

# 4. User Interaction:
Takes input from the user via the console for file name, content, and text replacement operations.

# Technology Used:
# 1. Java I/O Classes:
BufferedWriter and BufferedReader for efficient file writing and reading.
FileWriter and FileReader to handle file operations.

# 2. Java NIO (New I/O):
java.nio.file.Files and java.nio.file.Paths for reading and writing files with modern, efficient methods.

# 3. String Manipulation:
StringBuilder for efficient string construction during file reading.
String.replace() to handle text modifications.

# Key Insights:
# 1. Resource Management:
Use of try-with-resources ensures proper closure of I/O streams, preventing resource leaks.

# 2. Modularity:
Each operation (write, read, modify) is encapsulated in a separate method, promoting code reusability and readability.

# 3. Error Handling:
Comprehensive exception handling (IOException) ensures the program provides meaningful feedback even when operations fail.

# 4. File Content Manipulation:
Demonstrates a practical approach to modifying file content by leveraging Java's List and string methods.

# Final Output:
![image](https://github.com/user-attachments/assets/6cec4cbe-96dd-4cab-a9ca-612915f11935)
![image](https://github.com/user-attachments/assets/b499e87c-59aa-463b-a87f-d385366e3124)

