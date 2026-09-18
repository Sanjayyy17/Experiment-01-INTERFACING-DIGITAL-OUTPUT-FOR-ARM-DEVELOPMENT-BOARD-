# Experiment-01-INTERFACING DIGITAL OUTPUT FOR ARM DEVELOPMENT BOARD 
MOV [5004H], AX

MOV AX, 0FFFFH
MOV CX, 03H
DIV CX
MOV [5006H], AX

ret
~~~

## Output  :

<img width="1501" height="1066" alt="image" src="https://github.com/user-attachments/assets/d2b3da53-df64-44cf-b79e-d0304c1f6452" />


 program for logical operation:
 ~~~
 org 100h

MOV AX, 4456H
MOV BX, 0333H
AND AX, BX
MOV [5000H], AX

MOV AX, 0F345H
MOV CX, 2222H
OR AX, CX
MOV [5002H], AX

MOV AX, 1234H
NOT AX
MOV [5004H], AX

MOV AX, 0FFFFH
MOV BX, 0003H
AND AX, BX
NOT AX
MOV [5006H], AX

MOV AX, 00F0H
MOV CX, 0003H
OR AX, CX
NOT AX
MOV [5008H], AX

RET
 ~~~
## Output  :
<img width="1486" height="1073" alt="image" src="https://github.com/user-attachments/assets/a95d865a-1450-4443-a206-89d4bf56d41b" />



## Result :
Interfacing a digital output with ARM microcontroller is executed and the results are verified.


