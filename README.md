# IMAGE_ENCRYPTION

## Description
This is a simple Python script that encrypts and decrypts images using pixel manipulation. It applies an XOR (`^`) operation with a user-provided key to modify pixel values. The same key must be used for both encryption and decryption.

## Features
- Encrypt an image by altering pixel values.
- Decrypt an encrypted image to restore the original.
- Uses the `Pillow` and `NumPy` libraries for image processing.

## Requirements
Make sure you have Python installed and install the required dependencies using:
```sh
pip install pillow numpy
```
## Usage 
Run the script and follow the prompts
```sh
python image_encrypt.py
```
## Example
Encrypt an image
```sh
Enter 'encrypt' or 'decrypt': encrypt
Enter input image path: path/to/image.jpg
Enter output image path: path/to/encrypted_image.png
Enter an encryption key (0-255): 9
```
Decrypt an Image
```sh
Enter 'encrypt' or 'decrypt': decrypt
Enter input image path: path/to/encrypted_image.png
Enter output image path: path/to/decrypted_image.jpg
Enter an encryption key (0-255): 9
```
## How It Works
- The script reads an image and converts it into a NumPy array.
- Each pixel's value is modified using XOR (`^`) with the provided key.
- The modified pixel values are saved as a new image.
- Applying the same operation again with the same key restores the original image.

## Notes
- The encryption key must be between 0 and 255.
- Use the same key for encryption and decryption.
- The script works with JPG, PNG, and other common image formats.

## License
This project is open-source and available under the MIT License.




