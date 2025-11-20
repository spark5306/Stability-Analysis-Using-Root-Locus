# Stability Analysis using Root Locus
## Aim:
To analyse the stability of the system having open loop transfer function, G(S)=K/(S(S+5)(S+10)) using root locus and verify it using MATLAB. 
## Apparatus Required:
Computer with MATLAB software

## Theory:
<img width="910" height="1600" alt="image" src="https://github.com/user-attachments/assets/b373d11f-4ec1-4cc9-8ca1-14974bcfd07e" />
<img width="945" height="1600" alt="image" src="https://github.com/user-attachments/assets/7f9f32bc-7952-4faf-aa49-044bed98b67c" />
<img width="883" height="1600" alt="image" src="https://github.com/user-attachments/assets/6c15a54a-ab82-4c18-b2a5-7a459295979d" />


## Procedure:
	Open MATLAB software
	Open a new script file.
	Type the program.
	Save and Execute the program.
	Click on the crossing point of the root locus to find the value of K and poles at the crossing point.
	From the value of K, analyse the stability.

## Program: 
~~~
num=[1];
den=[1 15 50 0];
sys=tf(num,den);
rlocus(sys);
[k,poles]=rlocfind(sys)
~~~
## Output:

<img width="1919" height="1048" alt="Screenshot 2025-11-03 094240" src="https://github.com/user-attachments/assets/60a2354b-6432-4414-8684-cb018ffe3af5" />
<img width="1065" height="326" alt="image" src="https://github.com/user-attachments/assets/c1949846-a8c3-4caf-a5f0-8e0a4e08d702" />


## Result:
Thus the root locus for the given transfer function was drawn and verified using MATLAB. The conditions for stability is  0 < k < 755.9205
