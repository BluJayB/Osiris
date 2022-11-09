# Computer-Network-Security
programs from my CYEN 310 Computer network security class

## Osiris_binary.py program file
This is a Binary decoder python program that can auto detect and decode 7 or 8 bit binary encoded files
Syntax Example:
```
python Osiris_binary.py File_to_decode.txt
```
## Osiris_xor.py program file
This is a XOR encrypter and decrypter program that implements the XOR cryptography method

Encryption Syntax example:
```
python Osiris_xor.py < plaintext.txt > ciphertext.txt
```
Decryption Syntax Example:
```
pyhton Osiris_xor.py < ciphertext.txt > extracted_plaintext.txt
```
## steg.py steganography file
This a steganography program that can both store and retrieve hidden files either via bytes or bits
The required flags include: 
- (-r or -s) for retrieve or store
- (-B or -b) for Byte mode or bit mode
- (-o) for the byte offset
- (-i) for the interval
- (-w) for the wrapper file
- (-h) for the hidden file that will be stored, this is only used for storing mode

Syntax examples:
```
python steg.py -r -B -o1024 -i8 -wsecret_file.jpg > extracted_data.jpg

pyhton steg.py -s -b -o1024 -i8 -wnormal_file.jpg -hmy_secret_message.txt > secret_picture.jpg

```
## iter.bash steganography file
This is a bash file that does several iterations of steg.py. When using this file, the file steg.py must be in the same directory.
Note:
- This file should be used in a seperate sub folder/directory because it will cause a lot of clutter
- It takes one argument, the name of the file to retrieve data from
- If you want to change the values used for the offset and intervals, change to two lists in the file 

Syntax examples
```
bash iter.bash filename.txt
```
## Vigenere Website with a nice user interface
[Vigenere Decoder](https://www.dcode.fr/vigenere-cipher)
