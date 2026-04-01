# Digital-Signal-Processing--Convolution
## Aim:
                  To perform linear convolution using MAT LAB.
## Software Required:
MAT LAB R2012
## Algorithm:
Step 1: Open mat lab. Write the program.

Step 2: Read the first input sequence.

Step 3: Read the second impulse sequence.

Step 4: Plot the input sequences with x-label and y-label with suitable title. 

Step 5: Perform convolution for both the sequences using conv2() function.
  
Step 6: Plot the sequence with x-label and y-label with suitable title

Step 7: Terminate the program.

## PROGRAM: 
```
%Balaji v 212223050008

clc;
clear all; 
close all; 

% input sequence
a=-3;
x=[2,-1,2.7,2.6,3,6,3,5,-2];
n=a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');

%𝑥[𝑛]={2,3,-1,2.6,-2.3,4.2,3.6} and ℎ[𝑛]={3,2,9,-4.7,-1.8,2.4,1.6,5.7}
% -3 [2,3,-1,2.6,-2.3,4.2,3.6] 0 [3,2,9,-4.7,-1.8,2.4,1.6,5.7]

% impulse sequence
b=-0;
y=[3,2,9,-4.7,-1.8,2.4,1.6,5.7];
m=b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response')

% LINEAR CONVOLUTION
z=conv2(x,y);
n1=a+b:1:length (z)+a+b-1;
figure(3);
stem(n1,z);
xlabel('time');
ylabel('amplitude');
title('linear convolution');
```

## OUTPUT:
![WhatsApp Image 2026-02-10 at 7 54 56 PM](https://github.com/user-attachments/assets/77b5d981-79ff-44cf-a471-033810a96896)
![WhatsApp Image 2026-02-10 at 7 54 56 PM (1)](https://github.com/user-attachments/assets/f25af259-ec90-4d92-a7eb-38526b3b559b)
![WhatsApp Image 2026-02-10 at 7 54 56 PM (1)](https://github.com/user-attachments/assets/4ff4d50d-4758-4b3a-9b57-11159837f7a1)





## RESULT:
![WhatsApp Image 2026-04-01 at 10 57 31 AM](https://github.com/user-attachments/assets/d0415372-292f-4f6d-9916-b47e862437c1)



