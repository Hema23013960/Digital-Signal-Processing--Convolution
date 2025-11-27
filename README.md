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
clc; % clear screen
 clear all; % clear screen
 close all; % close all figure windows
% INPUT SEQUENCE
a=input('enter the starting x(n)');
x=input('enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');
% IMPULSE SEQUENCE
b=input('enter the starting h(n)');
y=input('enter the h(n) sequence');
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



## OUTPUT:
![WhatsApp Image 2025-10-15 at 13 53 51_7986c3cd](https://github.com/user-attachments/assets/7bb04395-8881-4fd4-a76f-7754de351d10)



## RESULT:
![WhatsApp Image 2025-11-27 at 17 53 33_2478847d](https://github.com/user-attachments/assets/68888996-3dfb-478f-a8c5-eeb80a2ade7a)


