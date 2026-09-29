# Image Steganography using LSB

This project demonstrates image steganography using Least Significant Bit (LSB) techniques for hiding and retrieving information in integers, grayscale images, and RGB images.

The program provides a menu-driven interface that allows the user to select different steganography operations. The project explores how information can be embedded into the least significant bits of digital data while preserving the main visual appearance of the cover image.

## Project Features

The program implements six steganography operations:

1. **Hide a Boolean value inside an integer**
   - A Boolean value (`True` or `False`) is stored by modifying the least significant bit of an integer.

2. **Retrieve a Boolean value from an integer**
   - The hidden Boolean value is recovered by reading the least significant bit.

3. **Hide and retrieve a binary image inside a grayscale image**
   - `grayscale.jpg` is used as the cover image.
   - `binary1.jpg` is embedded into the grayscale image using LSB modification.
   - The hidden binary image can then be extracted from the resulting image.

4. **Hide and retrieve three binary images inside an RGB image**
   - `rgb.jpg` is used as the cover image.
   - `binary1.jpg` is hidden in the Red channel.
   - `binary2.jpg` is hidden in the Green channel.
   - `binary3.jpg` is hidden in the Blue channel.
   - Each binary image is embedded into the least significant bit of its corresponding RGB channel.

5. **Hide and retrieve a grayscale image inside an RGB image**
   - `rgb.jpg` is used as the cover image.
   - `grayscale.jpg` is hidden across the RGB channels.
   - The grayscale image is then retrieved and displayed to verify the embedding and extraction process.

6. **Hide multiple bits of data per pixel**
   - The user selects the number of bits (`n`) to hide.
   - Binary data is provided as an integer.
   - The least significant `n` bits of each grayscale pixel are replaced with the provided data.

## Images Used

The `images/` directory contains the images used by the steganography experiments:

- `grayscale.jpg` – grayscale cover image
- `rgb.jpg` – RGB cover image
- `binary1.jpg` – binary image
- `binary2.jpg` – binary image
- `binary3.jpg` – binary image


## Implementation

The implementation is provided in `project.ipynb`. The notebook contains the functions for embedding and retrieving information using LSB-based steganography techniques.

## Authors

Mahmoud Tantawy  
James Adah
