# EC1421-19EC421-Analysis-and-Design-of-Analog-ICs
# DESIGN OF ACTIVE LOW PASS,HIGH PASS AND BAND PASS FILTERS USING OP-AMP 

## AIM: 

To design and obtain the frequency response of 
i) First order Low Pass Filter (LPF) 
ii) First order High Pass Filter (HPF) 
iii) Band pass filter
 
## APPARATUS REQUIRED

<img width="625" height="170" alt="image" src="https://github.com/user-attachments/assets/900fc8b3-3a8c-4208-bf52-98cc9e281e21" />

## THEORY
## LOW PASS FILTER 
 A LPF allows frequencies from 0 to higher cut of frequency, fH.  At fH the gain is 0.707 
Amax, and after fH gain decreases at a constant rate with an increase in frequency.  The gain 
decreases 20dB each time the frequency is increased by 10.  Hence the rate at which the gain 
rolls off after fH is 20dB/decade or 6 dB/ octave, where octave signifies a two fold increase in 
frequency.  The frequency f=fH is called the cut off frequency because the gain of the filter at this 
frequency is down by 3 dB from 0 Hz.  Other equivalent terms for cut-off frequency are -3dB 
frequency, break frequency, or corner frequency.
# HIGH PASS FILTER 
The frequency at which the magnitude of the gain is 0.707 times the maximum value of 
gain is called low cut off frequency.  Obviously, all frequencies higher than fL are pass band 
frequencies with the highest frequency determined by the closed –loop band width all of the op
amp. 
# BAND PASS FILTER 
A band pass filter has a pass band between two cutoff frequencies fH and fL such that fH > 
fL.  Any input frequency outside this pass band is attenuated.  There are two types of band-pass 
filters.  Wide band pass and Narrow band pass filters.  We can define a filter as wide band pass if 
its quality factor Q <10.  If Q>10, then we call the filter a narrow band pass filter.  A wide band 
pass filter can be formed by simply cascading high-pass and low-pass sections.  The order of 
band pass filter depends on the order of high pass and low pass sections.

## CIRCUIT DIAGRAM: 
## LOW_PASS
![WhatsApp Image 2025-11-27 at 13 41 11_d7a16b94](https://github.com/user-attachments/assets/de0f7f3f-0dff-4102-8e65-c774711c2748)

## HIGH-PASS
![WhatsApp Image 2025-11-27 at 13 41 22_a06a386a](https://github.com/user-attachments/assets/6a52ddb9-432f-45b5-bc0e-ea7b18da28f1)

## BAND-PASS
![WhatsApp Image 2025-11-27 at 13 41 49_59a3812c](https://github.com/user-attachments/assets/50dbc691-a3e4-4467-a120-fc4c88bbf734)

## MODEL GRAPH:
## LOW_PASS
![WhatsApp Image 2025-11-27 at 13 42 09_c5b2c3d3](https://github.com/user-attachments/assets/a8a8b1d5-285b-4ecd-813e-fed485fdaafc)

## HIGH-PASS
![WhatsApp Image 2025-11-27 at 13 42 34_ef9c764a](https://github.com/user-attachments/assets/63d0a4a8-c122-4ecd-832e-648209dcdccb)

## BAND-PASS
![WhatsApp Image 2025-11-27 at 13 42 53_aced3bd5](https://github.com/user-attachments/assets/d359d3ef-0aea-491e-aa96-6917f085cc80)

## PROCEDURE - (LPF & HPF): 
1. Connect the circuit as shown in the circuit diagram. 
2. Select the corresponding cut-off frequency (higher or lower) and determine the value of C&R. 
select the value of R1 & Rf depending on desired passband gain Af.. 
3. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
4. Tabulate the output voltage Vo with respect to different values of input frequency. 
5. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to  get approximately the same characteristic as shown in the model graph. 
# PROCEDURE:BAND PASS FILTER 
1. Select the lower and higher cut-off frequency and calculate the value of R & C for the given 
frequencies. 
2. Design for LPF & HPF separately and then combine the circuit by first placing the HPF 
followed by a LPF (i.e) HPF in series with LPF. 
3. Connect the circuit as shown in the circuit diagram. 
4. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
5. Tabulate the output voltage Vo with respect to different values of input frequency. 
6. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to get approximately the same characteristic as shown in the model graph

## DESIGN:LPF & HPF:

<img width="429" height="324" alt="image" src="https://github.com/user-attachments/assets/b0f0ac0a-3006-494c-9096-e91ae2d6e87c" />

# DESIGN: BAND PASS FILTER
Design a BPF to pass a band of 400Hz to 2KHz with a pass band gain of 4.  
1. Select the highest cut-off frequency of LPF as fH = 10 KHz and the lowest cut-off frequency 
of HPF as fL = 1 KHz.  
2. Design the HPF first by taking fL = 1KHz. Assume the value of C < 1μf.  
Let C = 0.1μf.  
3. Calculate R from the expression.  
Given: fH = 2KHz  = 1/ (2πR1C1) 
   Let C1 = 0.1 µF, R1 = 7.9 KΩ 
Given: fL = 400Hz  = 1/ (2πR2C2) 
   Let C2 = 0.1 µF, R2 = 39.8 KΩ 
  Pass band Gain=4 
   Now   Ao = 1 + (Rf / R1)  
               2-1=(Rf / Ri) 
                Ri = Rf 
                 Let  Ri = Rf = 10 KΩ
## TABULATION:
## LOW_PASS
![WhatsApp Image 2025-11-27 at 13 43 28_cb9f8892](https://github.com/user-attachments/assets/9c52e73d-e46a-420b-b926-e81c10f671f8)

## HIGH-PASS
![WhatsApp Image 2025-11-27 at 13 43 37_4ab357f1](https://github.com/user-attachments/assets/594b2c3d-b186-4e70-8086-fe884685e62e)

## BAND-PASS
![WhatsApp Image 2025-11-27 at 13 43 48_02e3a3e8](https://github.com/user-attachments/assets/80289833-e9eb-4377-95da-b38d87d1c8bc)

## GRAPH:
## LOW_PASS
![WhatsApp Image 2025-11-27 at 13 45 24_47ec55d6](https://github.com/user-attachments/assets/74beee68-6f3e-4dd5-9ef7-220b9ddff325)

## HIGH-PASS
![WhatsApp Image 2025-11-27 at 13 46 03_63507c11](https://github.com/user-attachments/assets/0072c5cc-fe48-44a1-8f42-48bf1223d813)

## BAND-PASS
![WhatsApp Image 2025-11-27 at 13 46 18_df700ae2](https://github.com/user-attachments/assets/6028a6b3-131d-44a3-a55c-8ce5a4e332b8)

 ## RESULTS:
Thus an Active Low pass, High pass and Band Pass Filters are designed and 
tested using op-amp IC 741. 

