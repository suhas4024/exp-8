Your code applies a Butterworth high-pass filter to an image, which allows high-frequency components to pass while attenuating low-frequency components. Here’s a summary of the steps:

Butterworth High-Pass Filter: The high-pass filter is defined similarly to the low-pass filter, but instead of attenuating high frequencies, it attenuates low frequencies. 
The filter uses the distance from the center of the frequency domain and the cutoff frequency to determine the filter strength.

DFT and Filtering: The code takes the Fourier Transform (FFT) of the image, applies the high-pass filter by multiplying the DFT of the image with the filter, 
and then applies the inverse FFT to get the filtered image back in the spatial domain.

Normalization: The filtered image is normalized so that pixel values are in the range [0, 255] for proper visualization and then converted to uint8 for image display.
