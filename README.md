# Pan Tompkins Algorithm with Python

The electrocardiogram (ECG or EKG) is the recording of the heart electrical activity (voltage). 
A normal rhythm ECG is composed of wave segments identified as: P-wave , QRS-complex, T-wave
and U-wave; each of these gives important information about the heart. Ih the QRS-complex, the
R-peak is the wave with the the greatest amplitude; identifying R-peaks,and using the time
interval between each one it is possible to calculate the heart rate, and detect arrhythmias.

The Pan-Tompinks algorithm is commonly used to detect R-peaks and compute heart rate. In this work we
implement the algorithm in Python, with the following general scheme: we start re-sampling ECG signals,
second we apply a band-pass filter to delete noise and a high-pass filter (derivative) to highlight
R-peaks; then we do a rectification via squaring the signal and apply a low-pass filter; finally we set
a threshold to detect peaks.

Additionally, the objective of this work is to evaluate the algorithm, in terms of detection accuracy,
with different parameter values in the different processing steps.