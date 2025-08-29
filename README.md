# EXPERIMENT--01-ALP-FOR-8086
Name : SANJEEVPRIYA K

Roll no : 212224040289

Date of experiment : 29.08.2025





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
```MOV CL,00
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
<img width="1920" height="1200" alt="Screenshot 2025-08-22 153800" src="https://github.com/user-attachments/assets/e9683f2f-e8d4-403c-b128-6ba78574d40d" />

 
## Subtraction   of 8 bit numbers  ALP 
```MOV CL,00
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
<img width="1920" height="1200" alt="Screenshot 2025-08-22 161026" src="https://github.com/user-attachments/assets/633bb628-c6df-482b-aef0-da6499b3ed0d" />

## Multiplication alp 
```MOV AX,[3001H]
MOV BX,[3003H]
MUL BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```  
 ## Output  
<img width="1920" height="1200" alt="Screenshot 2025-08-22 162707" src="https://github.com/user-attachments/assets/d7c13dc7-3593-4e31-9191-2ecdc26f9d2f" />


## Division alp 
```MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```


## Output  
<img width="1920" height="1200" alt="Screenshot 2025-08-22 162844" src="https://github.com/user-attachments/assets/06b5288d-4892-4aca-89e4-20ea8846117b" />

##program for logic operations

## AND
```MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT
```
## OUTPUT
<img width="1920" height="1200" alt="Screenshot 2025-08-29 100845" src="https://github.com/user-attachments/assets/d0840610-1ba3-47e3-b6ea-ca82e8a1e8ad" />

## OR
```MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT
```
## OUTPUT
<img width="1729" height="1017" alt="Screenshot 2025-08-29 101037" src="https://github.com/user-attachments/assets/ec23637e-54af-43bf-9d51-f3b3cfedde4c" />

## NOR
```MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## OUTPUT
<img width="1920" height="1200" alt="Screenshot 2025-08-29 104235" src="https://github.com/user-attachments/assets/ae069ea9-7f78-4a30-b2df-7850c7361e68" />

## NOT 
```MOV AX,[3001H]
NOT AX
MOV [3003H],AX
HLT
```
## OUTPUT
<img width="1920" height="1200" alt="Screenshot 2025-08-29 102312" src="https://github.com/user-attachments/assets/3f56b80d-edf0-4487-aaec-545daba668a4" />

## XOR

```MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT
```
## OUTPUT
<img width="1920" height="1200" alt="Screenshot 2025-08-29 101909" src="https://github.com/user-attachments/assets/77923d5c-6e84-4b83-b48e-3ac93e60ba75" />

## XNOR
```MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## OUTPUT

<img width="1920" height="1200" alt="Screenshot 2025-08-29 102140" src="https://github.com/user-attachments/assets/3f1470d5-66d1-4253-895f-d4f1af29ae0f" />




## Result :
  ALP on fundamental arithmetic and logical operations executed








