# Laboratory-Practice
# SPOS Practical Solutions

This repository contains solutions for System Programming and Operating System (SPOS) practicals, focusing on assembler, macro-processor, CPU scheduling, and page replacement algorithms.

## Problem Statements

### Q1: Pass 1 of a Two-Pass Assembler
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
