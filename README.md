# Steganography-repo
This is a Python implementation of the Discrete Wavelet Transform (DWT) that can be used to hide a message in an image. The DWT is a mathematical transform that decomposes an image into different frequency bands, allowing us to modify the image in a way that is less noticeable to the human eye. 

To hide a message in an image using the DWT, we first convert the message to a binary string. Then, we apply the DWT to the image to obtain the horizontal, vertical, and diagonal detail coefficients. We modify these coefficients by replacing the least significant bit of each coefficient with a bit from the binary message. By doing this, we can embed the binary message in the image without significantly altering its appearance.

The resulting image with the hidden message can then be saved as a file, and the message can be extracted by reversing the process. The receiver can apply the DWT to the image to obtain the modified coefficients, extract the least significant bit of each coefficient, and concatenate them to obtain the original binary message.

This implementation uses the PyWavelets library to perform the DWT and can be used as a basis for steganography applications or for educational purposes.
