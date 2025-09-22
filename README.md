# FACTORIAL-OF-A-NUMBER
# FACTORIAL OF A NUMBER USING 8051 (Keil)

## AIM
To write and execute an Assembly language program to perform the factorial of a number using 8051 Keil.

---

## APPARATUS REQUIRED
- Personal computer with Keil software

---

## ALGORITHM
1. **Start**
2. **Input**: Read the number `n`.
3. **Initialize**:
   - Set factorial to `1`.
   - Set `i` to `1`.
4. **Loop**: While `i` is less than or equal to `n`:
   - Multiply factorial by `i`.
   - Increment `i` by `1`.
5. **Output**: Store or print the value of factorial.
6. **End**

---

## FLOWCHART
<img width="506" height="525" alt="image" src="https://github.com/user-attachments/assets/f3b47187-6f0f-490c-8704-f2973cb2b276" />


---

## PROGRAM
```asm
ORG 0000H
MOV DPTR,#4500H
MOVX A,@DPTR
MOV R0,A
INC DPTR
ACALL FACTORIAL
MOVX @DPTR,A
SJMP THIN
FACTORIAL:DEC R0
CJNE R0,#01H,PRODUCT
SJMP THICK
PRODUCT:MOV B,R0
MUL AB
ACALL FACTORIAL
THICK: RET
THIN:RET
END

```
OUTPUT
<img width="1283" height="713" alt="image" src="https://github.com/user-attachments/assets/32fe825d-1c75-4c6f-825f-f26fd2b04a77" />
<img width="1321" height="636" alt="image" src="https://github.com/user-attachments/assets/07b5d047-19b1-496c-9b73-8c644eb87074" />
---
MANUAL CALCULATIONS
![WhatsApp Image 2025-09-22 at 19 01 16_803a4ebd](https://github.com/user-attachments/assets/9fb06f29-4366-476b-920f-aa9526fe0429)

---

RESULT

Thus, the factorial of a number was calculated and executed successfully using 8051 Keil.

---


