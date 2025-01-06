/**
 * A Java program to demonstrate reading, writing, and modifying text files.
 * This program provides methods for the following operations:
 * 1. Writing to a file.
 * 2. Reading from a file.
 * 3. Modifying a file's content.
 */

 import java.io.*;
 import java.nio.file.*;
 import java.util.*;
 
 public class FileOperation {
 
     // Method to write content to a file
     public static void writeFile(String fileName, String content) {
         try (BufferedWriter writer = new BufferedWriter(new FileWriter(fileName))) {
             writer.write(content);
             System.out.println("File written successfully.");
         } catch (IOException e) {
             System.err.println("Error writing to file: " + e.getMessage());
         }
     }
 
     // Method to read content from a file
     public static String readFile(String fileName) {
         StringBuilder content = new StringBuilder();
         try (BufferedReader reader = new BufferedReader(new FileReader(fileName))) {
             String line;
             while ((line = reader.readLine()) != null) {
                 content.append(line).append(System.lineSeparator());
             }
         } catch (IOException e) {
             System.err.println("Error reading from file: " + e.getMessage());
         }
         return content.toString();
     }
 
     // Method to modify content in a file
     public static void modifyFile(String fileName, String oldText, String newText) {
         try {
             // Read all lines from the file
             Path path = Paths.get(fileName);
             List<String> lines = Files.readAllLines(path);
 
             // Replace occurrences of oldText with newText
             for (int i = 0; i < lines.size(); i++) {
                 lines.set(i, lines.get(i).replace(oldText, newText));
             }
 
             // Write modified lines back to the file
             Files.write(path, lines);
             System.out.println("File modified successfully.");
         } catch (IOException e) {
             System.err.println("Error modifying file: " + e.getMessage());
         }
     }
 
     public static void main(String[] args) {
         Scanner scanner = new Scanner(System.in);
 
         System.out.println("Enter the file name (e.g., sample.txt):");
         String fileName = scanner.nextLine();
 
         // Writing to the file
         System.out.println("Enter content to write to the file:");
         String content = scanner.nextLine();
         writeFile(fileName, content);
 
         // Reading from the file
         System.out.println("Reading content from the file...");
         String fileContent = readFile(fileName);
         System.out.println("File Content:");
         System.out.println(fileContent);
 
         // Modifying the file
         System.out.println("Enter the text to be replaced:");
         String oldText = scanner.nextLine();
         System.out.println("Enter the new text:");
         String newText = scanner.nextLine();
         modifyFile(fileName, oldText, newText);
 
         // Display modified content
         System.out.println("Reading modified content from the file...");
         String modifiedContent = readFile(fileName);
         System.out.println("Modified File Content:");
         System.out.println(modifiedContent);
 
         scanner.close();
     }
 }
 
