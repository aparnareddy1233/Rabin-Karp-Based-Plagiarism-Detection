# Rabin-Karp Based Plagiarism Detection

## Description
This project implements a plagiarism detection system using the Rabin-Karp string matching algorithm. The algorithm detects whether a portion of text (pattern) exists in a larger document (text) using **hashing** and **rolling hash** techniques.

It is efficient for large documents and can be extended to compare multiple student assignments simultaneously.

## Features
- Detects plagiarism for a given text pattern.
- Uses rolling hash to slide through text efficiently.
- Minimizes character comparisons to save computation.
- Can be extended for multiple patterns or full document checks.

## How It Works
1. Compute hash of the **pattern**.
2. Compute hash of **each window** of text with the same length as pattern.
3. If hashes match, verify the substring character by character.
4. Use rolling hash to update the hash efficiently for the next window.
5. Output whether plagiarism is detected.

## Input & Output Example

**Input:**
Enter the text:
The quick brown fox jumps over the lazy dog
Enter the pattern to check:
brown fox

**Output:**
Plagiarism detected!

## Technologies Used
- Java
- Scanner for user input
- String handling and arithmetic for rolling hash

## How to Run
1. Clone the repository.
2. Open the project in your IDE (Eclipse, IntelliJ, VS Code).
3. Compile and run `PlagiarismDetection.java`.
4. Enter the text and pattern when prompted.

