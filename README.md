# EXPT 1b: Computation-of-DFT-using-FFT-ALGORITHM

## AIM
To perform and verify DFT using FFT-ALGORITHM by SCILAB.
## APPARATUS REQUIRED
PC installed with SCILAB
## PROGRAM 
### DFT FFT-ALGORITHM
```
clear;
clc;
close;
xn = [1 2 3 4];
n1 = 0:1:length(xn)-1;

subplot(2,2,1);
plot2d3(n1,xn);

xlabel('Time n');
ylabel('Amplitude');
title('Input Sequence');


Xk = fft(xn);
K1 = 0:1:length(Xk)-1;
magnitude = abs(Xk)

subplot(2,2,2);
plot2d3(K1, magnitude);

xlabel('frequency(Hz)');
ylabel('magnitude(gain)');
title('magnitude spectrum');

angle = atan(imag(Xk), real(Xk))

subplot(2,2,3);
plot2d3(K1, angle);

xlabel('frequency(Hz)');
ylabel('Phase');
title('Phase spectrum');

y = ifft(Xk);
n2 = 0:1:length(y)-1;

subplot(2,2,4);
plot2d3(n2, y);

xlabel('Time n');
ylabel('Amplitude');
title('Inverse FFT OF X(K)');
```
### CALCULATIONS:
<img width="1531" height="788" alt="image" src="https://github.com/user-attachments/assets/a098f10c-2dd9-4d15-954d-7ce8a5fcd74f" />
<img width="1015" height="1542" alt="image" src="https://github.com/user-attachments/assets/390fc28b-a0cb-4418-8a1e-2e9caed6c40d" />



### SAMPLE OUTPUT:
<img width="1600" height="1250" alt="image" src="https://github.com/user-attachments/assets/ab4e13ab-8ddd-4498-a1f5-0642b40e1b70" />



## RESULT:
Thus,  DFT using FFT-ALGORITHM for two given sequences were performed and its result was verified.

