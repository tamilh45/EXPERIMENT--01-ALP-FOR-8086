# EXPERIMENT--01-ALP-FOR-8086

### Name : TAMIL PAVALAN M

### Roll no : 212223110058

## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)







## Programs for arithmetic  operations

## Addition  of 8 bit ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
ADD AX,BX
JNC Loop
INC CL
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT    
```


## Output  
 <img width="1918" height="1003" alt="exp_1_addn" src="https://github.com/user-attachments/assets/79908061-fbd4-463f-b45a-29b9c0ea39a4" />

## Subtraction   of 8 bit numbers  ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
SUB AX,BX
JNC Loop
INC CL  
NOT AX
INC AX
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT
```

## Output  
<img width="1918" height="1013" alt="exp_1_sub" src="https://github.com/user-attachments/assets/d30cc50b-6e84-4246-a18f-2bef010b32a5" />

## Multiplication alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
MUL BX
MOV [3005H],AX
MOV [3007H],DX
HLT  
```

 ## Output  
<img width="1918" height="1017" alt="exp_1_mul" src="https://github.com/user-attachments/assets/293fb783-13ab-42a5-a21a-5e39deef1e87" />


## Division alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
## Output  
<img width="1918" height="1008" alt="exp_1_div" src="https://github.com/user-attachments/assets/d60b1c3e-c687-406e-a8fa-392a8b1248da" />

## AND operator
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT
```
## Output
<img width="1917" height="1017" alt="exp_1_and" src="https://github.com/user-attachments/assets/c1fc1157-dda9-4983-9d80-e554db0427e3" />


## OR operator
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT
```
## Output
<img width="1918" height="1012" alt="exp_1_or" src="https://github.com/user-attachments/assets/f6c17fd7-2259-4512-b9c5-6f101b860d59" />

## NOT operator
```
MOV AX,[3001H]
NOT AX
MOV [3003H],AX
HLT
```
## Output
<img width="1918" height="1003" alt="exp_1_not" src="https://github.com/user-attachments/assets/05d8fa47-85d2-4af4-99e4-2f3fd0b955bd" />

## NOR operator
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output
<img width="1918" height="1017" alt="exp_1_nor" src="https://github.com/user-attachments/assets/8a5237ff-b421-4e16-9b3b-91ac2771895a" />

## NAND operator
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output
<img width="1918" height="1012" alt="exp_1_nand" src="https://github.com/user-attachments/assets/c30c51cd-5782-4fee-b1ed-9886584735ff" />

## XOR operator
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT
```
## Output
<img width="1917" height="1017" alt="exp_1_xor" src="https://github.com/user-attachments/assets/9aa2437f-55a3-40b1-97f8-0569c02c59af" />

## XNOR operator
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output
<img width="1917" height="1015" alt="exp_1_xnor" src="https://github.com/user-attachments/assets/de6738f5-edf8-43b6-98b1-8d5cf42ebca0" />

## Result :

Thus, the programs have been written and executed for ALP on fundamental arithmetic and logical operations in the 8086 emulator.







