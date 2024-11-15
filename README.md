# Laboratory-Practice
# SPOS Practical Solutions

This repository contains solutions for System Programming and Operating System (SPOS) practicals, focusing on assembler, macro-processor, CPU scheduling, and page replacement algorithms.

## Problem Statements

Q1: Pass 1 of a Two-Pass Assembler
Implement pass 1 of a two-pass assembler with suitable data structures for a pseudo-machine.
START 100
A DS 3
L1 MOVER AREG, B
ADD AREG, C
MOVEM AREG, D
D EQU A+1
L2 PRINT D
ORIGIN L2+1
MOVEM AREG, ='34'
MOVEM AREG, ='14'
LTORG
STOP
MOVEM AREG, ='143'
MOVEM AREG, ='134'
B DC '19
C DC '17
END

Q2: Pass 2 of a Two-Pass Assembler
Implement pass 2 of a two-pass assembler for a pseudo-machine using the intermediate code generated in Pass 1.

Q3: Pass 1 of a Two-Pass Macro-Processor
Design suitable data structures and implement Pass-I of a two-pass macro-processor.
MACRO
M1 &X, &Y, &A=AREG, &B=
MOVER &A, &X
ADD &A, ='1'
MOVER &B, &Y
ADD &B, ='5'
MEND

MACRO
M2 &P, &Q, &U=CREG, &V=DREG
MOVER &U, &P
MOVER &V, &Q
ADD &U, ='15'
ADD &V, ='10'
MEND
START 100
M1 10, 20, &B=CREG
M2 100, 200, &V=AREG, &U=BREG
END

Q4: Pass 2 of a Two-Pass Macro-Processor
Implement Pass-II of a two-pass macro-processor, using the intermediate code generated in Pass 1.
CPU Scheduling Algorithms

Q5: First Come, First Serve (FCFS)
Write a program to simulate the FCFS CPU scheduling algorithm.

Q6: Shortest Job First (SJF) - Preemptive
Write a program to simulate the preemptive SJF CPU scheduling algorithm.

Q7: Priority Scheduling - Non-Preemptive
Write a program to simulate the Priority CPU scheduling algorithm (non-preemptive).

Q8: Round Robin (RR) - Preemptive
Write a program to simulate the Round Robin CPU scheduling algorithm with a fixed time quantum.

Q9: Page Replacement Algorithms
Write a program to simulate page replacement algorithms. Include:
FIFO (First-In-First-Out)
LRU (Least Recently Used)
Optimal Page Replacement


## To run your Java program from a text file in Eclipse IDE, follow these steps:

Step 1: Set Up Eclipse
Open Eclipse IDE.
If this is your first time opening it, select a workspace directory where your projects will be stored.

Step 2: Create a New Java Project
Go to File > New > Java Project.
Name the project (e.g., SPOS_Practicals).
Click Finish.

Step 3: Create a New Package (Optional)
Packages help organize files, but this step is optional.
In the Project Explorer on the left, right-click on the src folder inside your project.
Select New > Package.
Give it a name (e.g., com.example.spos) and click Finish.

Step 4: Create a New Java Class
Right-click on the package (or src folder if you didn’t create a package).
Select New > Class.
Give your class a name that matches the class name in your text file.
Example: If the main class in your text file is MainProgram, name this class MainProgram.
Ensure public static void main(String[] args) is checked if this is the main class.
Click Finish.

Step 5: Copy Code from Text File
Open your text file and copy the Java code.
Go back to Eclipse and open the class file you just created.
Paste the code into this class file, replacing any template code generated by Eclipse.

Step 6: Check for Any Issues
Eclipse should automatically highlight any errors. If there are errors, make sure your code’s structure matches Java conventions (such as matching class names and files).

Step 7: Run Your Program
Right-click on your Java class file in the Project Explorer.
Select Run As > Java Application.

Your program should now run, and any output will be displayed in the Console tab at the bottom of Eclipse.
