# FM

# EXP NO: 4	FREQUENCY MODULATION using SCILAB


**AIM:**

To write a program for Frequency Modulation using SCILAB and to observe and measure the frequency deviation and the modulation index of FM.


**APPARATUS REQUIRED:**

•	Computer with i3 Processor

•	SCI LAB

**THEORY:**

Frequency modulation is a type of modulation in which the frequency of the high frequency (carrier) is varied in accordance with the instantaneous value of the modulating signal.

***FREQUENCY DEVIATION f and MODULATION INDEX m f :***

The frequency deviation f represents the maximum shift between the  modulatedsignal
frequency, over and under the frequency of the carrier.

We define modulation index m f the ratio between f and the modulating frequency
m= f / fm 

***FREQUENCY MODULATION GENERATION:***

The circuits used to generate a frequency modulation must vary the frequency of a high frequency signal (carrier) as function of the amplitude of a low frequency signal (modulating signal). In practice there are two main methods used to generate FM.

**ALGORITHM:**

***1.	Define Parameters:***
 
 •	Fs: Sampling frequency.
 
 •	T: Duration of the signal.
 
 •	Fc: Carrier frequency.
 
 •	Fm: Frequency of the modulating signal.
 
 •	Beta: Modulation index, which controls the extent of frequency deviation.

***2.	Generate Signals:***

 •	Modulating signal: Sinusoidal signal used for modulation.
 
 •	Carrier signal: The high-frequency carrier signal.
 
 •	Modulated signal: FM modulated signal calculated by varying the carrier frequency according to the modulating signal.

***3.	FM Modulation:***

 •	Modulated signal is obtained by modulating the carrier signal with the modulating signal.
 

***4.	Visualization:***
 
 •	Plots the modulating signal, carrier signal, and FM modulated signal for analysis.



**PROCEDURE:**


•	Refer Algorithms and write code for the experiment.


•	Open SCILAB in System

•	Type your code in New Editor

•	Save the file

•	Execute the code

•	If any Error, correct it in code and execute again
Verify the generated waveform using Tabulation and Model Waveform

**MODEL GRAPH:**

<img width="512" height="365" alt="image" src="https://github.com/user-attachments/assets/acd787bd-5281-4f1b-802f-1aa39fac9189" />


**PROGRAM:**
~~~

fm=342;
Am=2.79;
fc=10*fm;
Ac=1.8*Am;
fs=10*fc;
t=0:1/fs:2/fm;
bp=3.54;
em=Am*cos(2*3.14*fm*t);
ec=Ac*cos(2*3.14*fc*t);
eFM=Ac*cos(2*3.14*fc*t+bp*sin(2*3.14*fm*t));
subplot(3,1,1);
plot(t,em);
subplot(3,1,2);
plot(t,ec);
subplot(3,1,3);
plot(t,eFM);

~~~


**OUTPUT WAVEFORM:**

<img width="1355" height="660" alt="exp-4 output" src="https://github.com/user-attachments/assets/c878e81f-f65f-40d5-9d8f-822926631b35" />



**TABULATION:**

<img width="3384" height="2003" alt="IMG_20261102_191937_edit_140174774551006 jpg" src="https://github.com/user-attachments/assets/59bcf8a3-645f-4d7b-afb0-4d43e03b41b1" />



**CALCULATION:**

<img width="2376" height="1110" alt="IMG_20261102_205241_edit_141679918308589 jpg" src="https://github.com/user-attachments/assets/f0d9e284-6832-4c69-8b4e-7057d153f580" />


<img width="2348" height="3490" alt="IMG_20261102_203626_edit_141410712048734 jpg" src="https://github.com/user-attachments/assets/c376d238-8f74-4a6b-98db-0f17b28e6d68" />





**RESULT:**

Thus, the frequency modulation is successfully done and the output is experimentally verified.


