# Arithmetic-operation-using-8086
# 8086 Assembly Language Programs for Arithmetic Operations

## AIM

To write and execute Assembly Language Programs to perform arithmetic operations for the 8086 microprocessor.

---

## APPARATUS REQUIRED

* Personal Computer with MASM Software

---

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
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,2000H
MOV CL,00H
MOV AX,[SI]
MOV BX,[SI+02H]
ADD AX,BX
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

| MEMORY LOCATION (INPUT) | MEMORY LOCATION (OUTPUT) |
| ----------------------- | ------------------------ |
|                         |                          |

#### Manual Calculations

(![WhatsApp Image 2025-09-14 at 17 52 03_8b01bf20](https://github.com/user-attachments/assets/fa875c99-8bf0-46c1-806c-577c84250825)
<img width="805" height="505" alt="image" src="https://github.com/user-attachments/assets/25432440-ac72-46a8-8d5b-d9f3d910c56e" />


## OUTPUT IMAGE FROM MASM SOFTWARE
<img width="777" height="481" alt="image" src="https://github.com/user-attachments/assets/e45960fc-4293-4650-a573-571ab1ce4b5e" />

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

| MEMORY LOCATION (INPUT) | MEMORY LOCATION (OUTPUT) |
| ----------------------- | ------------------------ |
|                         |                          |

#### Manual Calculations

![WhatsApp Image 2025-09-14 at 17 52 07_737c3df5](https://github.com/user-attachments/assets/8731b360-3191-4cde-83d6-8c71ab23a93e)


## OUTPUT SCREEN FROM MASM SOFTWARE
<img width="782" height="481" alt="image" src="https://github.com/user-attachments/assets/947387b2-5ebb-4755-bcff-871a294e4cf5" />
<img width="798" height="505" alt="image" src="https://github.com/user-attachments/assets/2b43019a-836a-4c90-b0a1-995068a25563" />

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

| MEMORY LOCATION (INPUT) | MEMORY LOCATION (OUTPUT) |
| ----------------------- | ------------------------ |
|                         |                          |

#### Manual Calculations

![WhatsApp Image 2025-09-14 at 17 55 40_1fe9604c](https://github.com/user-attachments/assets/0aafc31b-ae32-41e4-8450-893c86740312)


## OUTPUT SCREEN FROM MASM SOFTWARE
![WhatsApp Image 2025-09-14 at 18 25 14_84c21285](https://github.com/user-attachments/assets/4aa38acd-4b13-47e9-9ad7-59d2c984ac4c)

<img width="792" height="431" alt="image" src="https://github.com/user-attachments/assets/9a707420-318b-49ed-b283-3cc2acae3630" />

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

| MEMORY LOCATION (INPUT) | MEMORY LOCATION (OUTPUT) |
| ----------------------- | ------------------------ |
|                         |                          |

#### Manual Calculations

![WhatsApp Image 2025-09-14 at 17 52 09_bda9421c](https://github.com/user-attachments/assets/916c5cc6-787d-4c6d-a55e-421075b69888)

## OUTPUT FROM MASM SOFTWARE
![WhatsApp Image 2025-09-14 at 18 25 15_3386397f](https://github.com/user-attachments/assets/1efece6b-d3e3-42ae-9f54-5f95e2ce4818)


<img width="792" height="427" alt="image" src="https://github.com/user-attachments/assets/a57be435-c99e-4c1c-bbca-704a63d49871" />


## RESULT

Thus, the Assembly Language Programs for 8086 to perform arithmetic operations (Addition, Subtraction, Multiplication, and Division) using both direct and indirect methods were successfully written and executed using MASM.

