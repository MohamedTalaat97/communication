# communication
# Matlab Simulink project BPSK, QPSK, FSK, QAM(16-64) with an AWGN environment and raised cos


- Simulation Steps:
  - AWGN: Eb/No= 10 db 
  - RandomIntegerGeneration: samplesPerFrame=100 
  - sourceOfInitialSeed=parameter
  - simulation time 1000000
  - in ToWorkspace block (simout) set variable name = ber,save format = array and save 2-D signals = 2-D array
  - open bertool
  - thoeratical set Eb/No range = -10:10 
  - in monte carlo set Eb/No range = -10:1:10 with step 1
  - set no. of bite to 1e4 
  
# Binary Phase Shift Keying (BPSK)
It is a digital modulation technique. 
binary 1 and binary 0 are represented by different carrier phases each is 180 degree apart.
The simplest BPSK scheme uses two phases to represent the two binary digits and is known as binary phase-shift keying.

- BPSK Simulation
  - RandomIntegerGeneration:set size = 2
## scatter plot and ber diagram 
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/bpsk/bbsk%20before%20noise.PNG)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/bpsk/bpsk%20after%20noise.PNG)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/bpsk/bpsk%20ber.png)

## scatter plot and ber diagram (raised cos)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/raised%20cosine/bpsk/bpsk%20before%20raised.PNG)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/raised%20cosine/bpsk/bpsk%20raised%20after%20.PNG)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/raised%20cosine/bpsk/bpsk%20raised.PNG)  
  
  
# Quadrature Phase Shift Keying (QPSK)
It is a digital modulation technique.
QPSK is bandwidth efficient as each signal point represents two bits. 
For example, instead of a phase shift of 180 degree, as allowed in BPSK, 
a common encoding technique, known as QPSK uses phase shifts of multiples of 90 degrees.

- QPSK Simulation
  - RandomIntegerGeneration:set size = 4
## scatter plot and ber diagram 
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/qpsk/qpsk%20before%20noise.PNG)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/qpsk/qpsk%20after%20noise.PNG)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/qpsk/qpsk.png)  

## scatter plot and ber diagram (raised cos)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/raised%20cosine/qpsk/qpsk%20before%20raised.PNG)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/raised%20cosine/qpsk/qpsk%20raised%20after.PNG)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/raised%20cosine/qpsk/qpsk%20raised.PNG)  
  
  

#Quadrature Amplitude Modulation (QAM) -16
This is also antoher modulation scheme but carry information in amplitude and in phase (only two phases). It uses two carriers sin and cos and recived signal with differnt amplitudes. bits per symbol = 4.

- For QAM-16 Simulation
  - RandomIntegerGeneration:set size = 16
  - In modualtor and demodualtor: M-ary number =16
  
## scatter plot and ber diagram 
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/qam16/qam%20before.PNG)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/qam16/qam%2016%20after.PNG)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/qam16/qam.png)  
  
 ## scatter plot and ber diagram (raised cos)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/raised%20cosine/qam%2016/qam%20raised%20before.PNG)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/raised%20cosine/qam%2016/qam%20after%20raised.PNG)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/raised%20cosine/qam%2016/qam%20raised.PNG)  


#Quadrature Amplitude Modulation (QAM) -64

- QAM-64 Simulation
  - RandomIntegerGeneration:set size = 64
  - In modualtor and demodualtor: M-ary number = 64
  
## scatter plot and ber diagram 
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/qam64/qam64%20before.PNG)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/qam64/qam64%20after%20noise.PNG)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/qam64/qam64.png)  

## scatter plot and ber diagram (raised cos)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/raised%20cosine/qam64/qam64%20raised%20after.PNG)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/raised%20cosine/qam64/qam64%20raised.PNG) 

# Frequency Shift Keying (FSK)
FSK stands for Frequency-shift keying
allows digital information to be transmitted by changes or shifts in the frequency of a carrier signal, 
most commonly an analog carrier sine wave. There are two binary states in a signal, zero (0) and one (1), each of which is represented by an analog wave form.
This binary data is converted by a modem into an FSK signal, which can be transmitted via telephone lines, fiber optics or wireless media.
FSK is commonly used for caller ID and remote metering applications.
FSK is also known as frequency modulation (FM).

- FSK Simulation
  - RandomIntegerGeneration:set size = 2.
  
## scatter plot and ber diagram 
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/fsk/fsk%20before.PNG)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/fsk/fsk%20after%20.PNG)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/fsk/fsk-d.png)  


## scatter plot and ber diagram (raised cos)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/raised%20cosine/fsk/fsk%20raised%20before.PNG)
![bpsk](https://github.com/mohameDMEDO97/communication/blob/master/raised%20cosine/fsk/fsk%20raised%20beofre.PNG)
  
  
