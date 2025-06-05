# Task-4-DIGITAL-FILTER-DESIGN

*COMPANY*: CODTECH IT SOLUTIONS 

*NAME*: Sujal Chavan

*INTERN ID*: CT04DF1863

*DOMAIN*: VLSI

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTOSH

# Description of the Task

In this task, a digital Finite Impulse Response (FIR) filter was designed and simulated using MATLAB. FIR filters are a class of linear time-invariant filters widely used in digital signal processing (DSP) due to their inherent stability and linear phase characteristics. The objective was to design a low-pass FIR filter using the window method, apply it to a noisy composite signal, visualize its characteristics, and analyze its performance.

Filter Design Methodology

The design approach adopted was the window method, which is a classical technique for FIR filter design. In this method, an ideal filter response is truncated and smoothed using a window function to reduce the side lobes and ripple in the frequency domain. Specifically, we designed a low-pass filter using the fir1 function in MATLAB with a Hamming window. This window is commonly used because of its good trade-off between main lobe width and side lobe attenuation.

The key parameters defined for the filter were:

Sampling Frequency (fs): 1000 Hz

Cutoff Frequency (fc): 100 Hz

Filter Order (N): 50

The cutoff frequency was normalized relative to the Nyquist frequency (fs/2), resulting in a normalized cutoff of Wn = 0.2. The fir1 function generated the filter coefficients (b), and these coefficients define the impulse response of the FIR filter.

Simulation and Signal Processing

To evaluate the filter, a synthetic test signal was generated consisting of two sinusoidal components:

A 50 Hz sine wave (which lies in the passband)

A 200 Hz sine wave (which lies in the stopband)

To simulate real-world conditions, random Gaussian noise was added to the signal. This noisy signal was then passed through the designed FIR filter using the filter function in MATLAB. The performance of the filter was evaluated in both the time domain and frequency domain.

Time domain plots were generated to show:

The original clean signal

The noisy input signal

The output signal after filtering

In the frequency domain, Fast Fourier Transform (FFT) was applied to both the noisy and filtered signals to visualize how effectively the FIR filter attenuated the high-frequency noise and the 200 Hz component.

Performance Analysis

The performance of the FIR filter was quantitatively assessed using three key metrics:

Stopband Attenuation: The magnitude response around 200 Hz was extracted, and it showed an attenuation of around -50 dB, confirming that the high-frequency component was effectively suppressed.

Passband Ripple: The filter exhibited minimal ripple around 50 Hz (the desired frequency), with the ripple being well below 0.01, indicating excellent performance in the passband and preserving the desired signal.

Signal-to-Noise Ratio (SNR): The SNR before filtering was lower due to the added noise. After filtering, the SNR significantly improved, demonstrating the FIR filter's ability to clean the signal by attenuating the unwanted noise and high-frequency interference.

Conclusion

This exercise clearly demonstrated the practical application of FIR filters in digital signal processing using MATLAB. The filter design was intuitive and implemented using standard functions like fir1, filter, and freqz. The simulation effectively showcased the filter's ability to suppress unwanted high-frequency components while preserving the desired signal. The visualization of impulse response, frequency response, and time-domain signals helped understand the filter behavior comprehensively.

The results affirmed that FIR filters designed with window methods like Hamming are highly efficient for applications requiring linear phase response and sharp cut-off characteristics. Moreover, the FIR filter’s performance in terms of stopband attenuation, minimal passband ripple, and SNR improvement indicates that it is suitable for real-world digital filtering applications such as audio processing, biomedical signal filtering, and communications.

# OUTPUT

![Image](https://github.com/user-attachments/assets/60e3ef19-3268-40fd-8acc-5a3e2b03766b)

![Image](https://github.com/user-attachments/assets/754c52c1-07e0-4f0a-9cf9-4cbc24bfe397)

![Image](https://github.com/user-attachments/assets/49e1475d-533d-41d4-bf14-70bf7943f562)

![Image](https://github.com/user-attachments/assets/4cdf48d3-ed87-4c1f-ae6f-4760a11ad78c)

![Image](https://github.com/user-attachments/assets/201a15b1-b073-4fb5-a38e-40a1d6e777d2)
