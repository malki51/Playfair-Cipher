Playfair Cipher in Python
The Playfair Cipher is a digraph substitution cipher that encrypts pairs of letters instead of individual letters. It was used for tactical purposes during various historical events , including World War I and World War II .Here’s how you can implement it in Python:
Usage
1.	Clone this repository or download the Playfair Cipher.py file.
2.	Run the program using Python 3:
3.	Playfaircipher.py
4.	Follow the prompts to input your key and plaintext message.
Implementation Details

•	The key square is a 5x5 grid of unique alphabets (excluding ‘J’). If the plaintext contains ‘J’, it is replaced by ‘I’.

•	The plaintext is split into pairs of two letters (digraphs). If there’s an odd number of letters, a ‘Z’ is added to the last letter.

•	Rules for encryption:

o	If both letters are in the same column, take the letter below each one.

o	If both letters are in the same row, take the letter to the right of each one.

o	If neither rule applies, form a rectangle with the two letters and take the letters on the horizontal opposite corner of the rectangle.

Example
Suppose you want to encrypt the plaintext “security”:

•	After splitting: ‘se’ ‘cu’ ‘ri’ ‘ty’

•	Encrypted text: “mkocpecp”

