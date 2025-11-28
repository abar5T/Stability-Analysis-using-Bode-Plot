# Stability-Analysis-using-Bode-Plot
## Aim:
To analyse the stability of the system having open loop transfer function, G(S)=1/(S(1+0.5S)(1+0.1S)) using bode plot and verify it using MATLAB. 
## Apparatus Required:
Computer with MATLAB software

## Theory:
![WhatsApp Image 2025-11-27 at 21 39 10_983ec10b](https://github.com/user-attachments/assets/39e7a43d-42a7-4bba-8335-5fd5fda5f6f6)
![WhatsApp Image 2025-11-27 at 21 39 39_217ec39c](https://github.com/user-attachments/assets/bc6e686b-d6b4-447c-bcc1-a82e4bce0269)
![WhatsApp Image 2025-11-27 at 21 40 18_11eaf2cd](https://github.com/user-attachments/assets/9c43624a-8aa1-4dac-8461-0fc677f72e47)
![WhatsApp Image 2025-11-27 at 21 42 08_163efbe4](https://github.com/user-attachments/assets/9b43516d-f389-4d3b-baa4-55e4a86fd239)



## Procedure:
	Open MATLAB software
	Open a new script file.
	Type the program.
	Save and Execute the program.
	Determine the gain crossover frequency, phase cross over frequency, gain margin and phase margin.
	Also determine the stability.

## Program: 
num=1 <br>
den=[0.05 0.6 1 0] <br>
sys=tf(num,den) <br>
bode(sys) <br>
grid on <br>
[Gm Pm Wpc Wgc]=margin(sys) <br>
if(Wpc>Wgc) <br>
    disp('stable') <br>
elseif(Wpc == Wgc) <br>
    disp('marginally stable') <br>
else <br>
    disp('unstable') <br>
end <br>

## Output:
![exp05](https://github.com/user-attachments/assets/041ca36c-6e16-4636-bdb5-483c30e8556c)


## Result:
Thus the bode plot for the given transfer function was drawn and verified using MATLAB. <br>
Gain margin = 12.0 <br>
Phase Margin = 60.42 <br>
Gain crossover frequency = 0.907<br>
Phase crossover frequency = 4.4721 <br>
The system is  stable
