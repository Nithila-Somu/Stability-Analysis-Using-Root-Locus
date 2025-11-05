# Stability Analysis using Root Locus
## Aim:
To analyse the stability of the system having open loop transfer function, G(S)=K/(S(S+5)(S+10)) using root locus and verify it using MATLAB. 
## Apparatus Required:
Computer with MATLAB software

## Theory:
![WhatsApp Image 2025-11-05 at 08 58 32_b77d5ee9](https://github.com/user-attachments/assets/eac65cde-32af-44e3-b635-2cd30439d1d6)
![WhatsApp Image 2025-11-05 at 08 58 46_75e53038](https://github.com/user-attachments/assets/44996e22-9132-4c22-90ca-caf11d2454c5)
![WhatsApp Image 2025-11-05 at 08 58 59_3eefc6df](https://github.com/user-attachments/assets/e82c05c9-be38-45d0-ba6c-826278115412)

![WhatsApp Image 2025-11-05 at 08 59 05_b30dcec7](https://github.com/user-attachments/assets/e9243526-0b02-4cc8-a561-2e72e35e38c5)






## Procedure:
	Open MATLAB software
	Open a new script file.
	Type the program.
	Save and Execute the program.
	Click on the crossing point of the root locus to find the value of K and poles at the crossing point.
	From the value of K, analyse the stability.

## Program: 
```
num = [1];
den = [1 15 50 0];
sys = tf(num, den);       
rlocus(sys);              
[k poles] = rlocfind(sys);

```



## Result:

![csexp4](https://github.com/user-attachments/assets/b95b8502-bd6a-49a0-82bc-debcbd4f8f1e)



Thus the root locus for the given transfer function was drawn and verified using MATLAB. The conditions for stability is k<741
