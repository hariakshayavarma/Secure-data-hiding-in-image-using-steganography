# Secure-data-hiding-in-image-using-steganography
# Image-Based Steganography

This repository provides a *lightweight and efficient* implementation of *image-based steganography* using Python and OpenCV. It enables users to *hide and retrieve secret messages* within an image while ensuring a simple passcode-based authentication system.

## Features
- Hide and retrieve secret messages inside images with minimal distortion.
- Passcode authentication for controlled access to the hidden data.
- Simple and easy-to-use interface with minimal dependencies.
- Uses pixel modification for message embedding.

## Requirements
Ensure you have the following dependencies installed before running the scripts:


pip install opencv-python


## Usage

### Encryption (Hiding a Message)
This script embeds a secret message inside an image by modifying pixel values.

Run the script:

python encrypt.py

#### Steps:
1. Enter the secret message you wish to hide.
2. Provide a passcode for security.
3. The encrypted image is generated and saved as encryptedImage.jpg.

### Decryption (Retrieving the Message)
This script extracts the hidden message from the encrypted image.

Run the script:
bash
python decrypt.py

#### Steps:
1. Enter the passcode used during encryption.
2. If the passcode matches, the hidden message is displayed.

## Files in Repository
- encrypt.py - Script to embed a message inside an image.
- decrypt.py - Script to retrieve the hidden message from an image.
- sample.jpg - Sample image for testing purposes.

## Important Notes
- The passcode serves as authentication but does *not* encrypt the message. Future updates could integrate encryption techniques like AES for enhanced security.
- Ensure the image has enough pixel capacity to store the entire message to avoid data loss.
- Direct pixel modifications may introduce slight distortions; for improved security, *LSB (Least Significant Bit) encoding* or *cryptographic encryption* can be incorporated.
- This method is *not suitable for high-security applications* but works well for basic steganographic needs.

## Future Enhancements
- Implement *LSB-based encoding* to minimize visible distortions.
- Integrate *AES encryption* to enhance message security.
- Improve error handling for better robustness.
- Optimize pixel traversal to reduce artifacts in modified images.

## License
This project is licensed under the *MIT License*.



## Contributions
Contributions are encouraged! Feel free to submit *issues* or *pull requests* for enhancements.

---
### Author: [P.Hari Akshaya Varma]  
GitHub: [hariakshayavarma]
