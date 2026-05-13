# Arithmetic-operation-using-8086
# 8086 Assembly Language Programs for Arithmetic Operations

## AIM

To write and execute Assembly Language Programs to perform arithmetic operations for the 8086 microprocessor.

---

## APPARATUS REQUIRED

* Personal Computer with MASM Software


## 1. ADDITION

#### Algorithm

1. Initialize memory location in HL register.
2. Store 1st data.
3. Increment HL to enter 2nd data.
4. Move 2nd number to accumulator.
5. Decrement HL.
6. Add value in memory with accumulator.
7. Store result.
8. Stop.


## FLOW CHART
<img width="707" height="1024" alt="image" src="https://github.com/user-attachments/assets/b5a7062d-e294-47cd-9683-a40de25e82de" />


#### Program

```asm
CODE SEGMENT
ASSUME CS:CODE, DS:CODE
ORG 1000H
MOV CL,00H
MOV AX,1234H
MOV BX,1234H
ADD AX,BX
JNC L1
INC CL
L1:MOV SI,1200H
MOV [SI],AX
MOV [SI+2],CL
MOV AH,4CH
INT 21H
CODE ENDS
END
```

#### Output Table

<img width="641" height="331" alt="image" src="https://github.com/user-attachments/assets/ad210503-f230-4644-ba1a-a4d7d4243792" />


#### Manual Calculations

<img width="267" height="182" alt="image" src="https://github.com/user-attachments/assets/e0dbdec6-2b6e-48ca-b8a3-774d15d1f477" />

## OUTPUT IMAGE FROM MASM SOFTWARE

<img width="734" height="509" alt="image" src="https://github.com/user-attachments/assets/c0a52128-86eb-4a06-865a-59a97feba9a0" />


## 2. SUBTRACTION

#### Algorithm

1. Initialize memory and store 1st data.
2. Increment to get 2nd data.
3. Move 2nd data to accumulator.
4. Subtract memory content.
5. Store result.

## FLOWCHART

<img width="578" height="797" alt="image" src="https://github.com/user-attachments/assets/564c3c7a-33ce-4a1c-8920-beb5c24b9b47" />


#### Program
```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,2000H
MOV CL,00H
MOV AX,[SI]
MOV BX,[SI+02H]
SUB AX,BX
JNC L1
INC CL
L1:
MOV [SI+04H],AX
MOV [SI+06H],CL
MOV AH,4CH
INT 21H
CODE ENDS
END
```


#### Output Table

<img width="646" height="277" alt="image" src="https://github.com/user-attachments/assets/a663e3ff-c443-4083-b959-5273cad87c0b" />

#### Manual Calculations


<img width="259" height="141" alt="image" src="https://github.com/user-attachments/assets/b68e88fe-09cc-41a9-b6a1-3b30e6cf93ff" />

## OUTPUT SCREEN FROM MASM SOFTWARE

<img width="737" height="499" alt="image" src="https://github.com/user-attachments/assets/3dbf4612-ddf4-4c59-b4a8-2521ef8a318c" />

## 3. MULTIPLICATION

#### Algorithm

1. Initialize memory and store operands.
2. Move operands to registers.
3. Multiply.
4. Store result.

##FLOWCHART

<img width="569" height="906" alt="image" src="https://github.com/user-attachments/assets/88be88ff-2896-4a88-b73d-84ccffd2fcf9" />

#### Program

```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,2000H
MOV DX,0000H
MOV AX,[SI]
MOV BX,[SI+02H]
MUL BX
MOV [SI+04H],AX
MOV [SI+06H],DX
MOV AH,4CH
INT 21H
CODE ENDS
END
```

#### Output Table

<img width="629" height="337" alt="image" src="https://github.com/user-attachments/assets/2a206641-5b65-495d-beca-5b0072a66dab" />

#### Manual Calculations

<img width="631" height="317" alt="image" src="https://github.com/user-attachments/assets/0850282c-491c-45a2-a90e-b9d5af7b2d1c" />

## OUTPUT SCREEN FROM MASM SOFTWARE

<img width="734" height="521" alt="image" src="https://github.com/user-attachments/assets/2c9bfb16-1094-475d-a21c-da1de93e09de" />

## 4. DIVISION

#### Algorithm

1. Load memory location of operands.
2. Perform division.
3. Store result.

   ## FLOWCHART
<img width="1065" height="802" alt="image" src="https://github.com/user-attachments/assets/25b4a483-0d42-494b-8639-1af3ea17191b" />


#### Program

```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,2000H
MOV DX,0000H
MOV AX,[SI]
MOV BX,[SI+02H]
DIV BX
MOV [SI+04H],AX
MOV [SI+06H],DX
MOV AH,4CH
INT 21H
CODE ENDS
END
```

#### Output Table

<img width="639" height="291" alt="image" src="https://github.com/user-attachments/assets/86da03ac-a22f-4509-a1c2-ef1942f0497c" />

#### Manual Calculations

<img width="308" height="184" alt="image" src="https://github.com/user-attachments/assets/9ebc9641-1429-4b58-b954-5b659520ed7b" />

## OUTPUT FROM MASM SOFTWARE

<img width="737" height="509" alt="image" src="https://github.com/user-attachments/assets/8f11afcb-2dde-4079-be60-1f615b1a2405" />



## RESULT

Thus, the Assembly Language Programs for 8086 to perform arithmetic operations (Addition, Subtraction, Multiplication, and Division) using both direct and indirect methods were successfully written and executed using MASM.
.



.




.



.





.




.









.













.














.





.












