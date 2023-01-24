# Tucil1_13521088

The 24 card game is an arithmetic card game with the aim of finding ways to operate 4 random numbers so that the final result is 24. The cards used have 13 values: A, 2, 3, 4, 5, 6, 7, 8, 9, 10, J, Q, K. The A, J, Q, K counted as 1, 11, 12, 13, consecutively. The operators that can be used are +, -, *, /, and ().

This program provide all the posible solutions to the 24 card game from 4 card values inputed or randomly generated. This program used Brute Force algorithm to generate all the possible solutions and is written in C++ languange.

## Table of Contents

- [Background](#background)
- [Program's Features](#program's-features)
- [Requirements/Installations](#requirements/installations)
- [Tutorial](#tutorial)
- [Repository's Structure](#repository's-structure)
- [Author](#author)

## Background
This program was made to fulfill Tugas Kecil IF2211 Strategi Algoritma Semester II tahun 2022/2023, Program Studi Teknik Informatika, Sekolah Teknik Elektro dan Informatika, Institut Teknologi Bandung

## Program's Features
- [x] Program can read user input or randomly generate card numbers.
- [x] Program output all of the possible solution(s) to the 24 games correctly.
- [x] Program output the ammount of solution(s) found correctly.
- [x] Program output the excecution time of the solution finding algorithm.
- [x] Program can save the solution(s) into a txt file.

## Requirements/Installations
This program used headers iostream, unordered_set, fstream, and other functions in the C++ STL.

g++ Compiler Installation: `$ sudo apt install g++`

## Tutorial

1. Compile & Run the program.
```bash
g++ main.cpp -o main.out
./main.out
```

2. Input an option.
```bash
Choose an option (1/2/3):
1. Generate random cards
2. Input my own cards
3. Exit
```

3. Input the card numbers if you choose option 2, or else random cards are automatically generated.
```bash
Format: [A/1, 2, 3, 4, 5, 6, 7, 8, 9, 10, J, Q, K]
ex:
1: A
2: 2
3: J
4: K
```

3. The solutions will be generated.
```bash
ex:
24 solution(s) found
4*(12-(1+5))  4*(12-(5+1))  (12-(5+1))*4  12*(1+(5-4))
12*((1-4)+5)  ((12-1)-5)*4  4*((12-5)-1)  (5+(1-4))*12
(1+(5-4))*12  12*((5+1)-4)  (5-(4-1))*12  12*(1-(4-5))
12*((5-4)+1)  12*(5+(1-4))  ((1-4)+5)*12  (12-(1+5))*4
(1-(4-5))*12  ((5+1)-4)*12  12*((1+5)-4)  ((1+5)-4)*12
((5-4)+1)*12  4*((12-1)-5)  ((12-5)-1)*4  12*(5-(4-1))  

Time taken to search the solution is : 0.000624 sec
```
4. Input y if you want to save the solution into file, then input the file name, or input n if you don't want to save.
```bash
*o*o*o*o*o*o*o*o*o*o*o*o*o*o*o*o*o*o*o*o

Do you want to save the solution(s) (y/n)?  y 
Filename (without extension): test2
'../test/test2.txt' successfully saved!

*o*o*o*o*o*o*o*o*o*o*o*o*o*o*o*o*o*o*o*o
```

5. If you choose to save, the file will be located at the test folder.

## Repository's Structure
```bash
.
│   README.md
|
├───doc
|    └──Tucil1_K2_13521088_Puti Nabilla Aidira.pdf         
├───src
|    └──main.cpp    
├───bin
|    └──main.out  
└──test
     └──test1.txt
     └──test2.txt
     └──test3.txt
     └──test4.txt
     └──test5.txt            
```

## Author
Puti nabilla Aidira (13521088)