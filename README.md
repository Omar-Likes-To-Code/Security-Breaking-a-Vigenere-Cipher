# Security-Breaking-a-Vigenere-Cipher
Vigenère Cipher Cracker
This Python script implements an algorithm to break the Vigenère Cipher using the Index of Coincidence (IC) method. The Vigenère Cipher is a classical polyalphabetic substitution cipher, where the key is repeated to encrypt the plaintext. The cracking algorithm uses the concept of IC to estimate the most probable key length and subsequently decrypt the ciphertext.

Features
Calculates the Index of Coincidence (IC) for a given text.
Divides the ciphertext into cosets based on a guessed key length.
Estimates the most probable key length by calculating the average IC for each possible key length.
Outputs the probable key length.
Installation
This script requires Python 3.x. No additional libraries are needed.

To run the script, simply execute it with Python:

bash
Copy code
python vigenere_cipher_cracker.py
Usage
Input: The ciphertext string.
Output: The probable key length.
python
Copy code
s0 = "RSTCSJLSLRSLFELGWLFIISIKRMGL"
s1 = "OICPWZXZEVLGCLNFSYPGALPXWZJTEGALPCSIIWDHOIECCBFWPAHOPCGALPCCBROASNWTYHOIDBIHVPSCSIDEVLSYPGDLZDSLXSTBNWOTTMICPBAPJEVLCLCSUSEQCUHZQFBPPDOUHESSFLLGSUSCPGWINETVVESSZXLEIZUFZMVYNLBXYZESALPXRPWLRFLIHTHOXSPANPZCWMCZCJPPTQMALPXOISFEHOIZYZFXSTBNCZFQHRYZHKSTDWNRZCSALPXPLGLFGLXSPMJLLYULXSTBNWESSFTFDVALPSITEYCOJIQZFDECOOUHHSWSIDZALQLJGLIESSTEDEVLGCLNFSYPGDIDPSNIYTIZFPNOBWPEVLTPZDSIHSCHVPNFHDJPBVYRSHVXSTBRXSPMJEYNVHRRPHOIHZFSHLCSALPZBLWHSCKS"
s2 = "VVVXSQWPSNJMUMJOKKLGFQAVEXAHWRVTMFXVVRKAJTVMFLOPHYWJDSTXKAGFVVTPHKYEPPJOKPSWACJVSIGGVOLXLVMQPVCMGOGMFLAKENVRMIUAKTKVHIXCFJZRAHWFHLIUMHCIRFWGFOETIUNEQVJWEHOSJWVQFYWKYMPGQHWISOPKHYFYV"

key_length_s0 = crack(s0)
key_length_s1 = crack(s1)
key_length_s2 = crack(s2)

print("Probable key length for s0:", key_length_s0)
print("Probable key length for s1:", key_length_s1)
print("Probable key length for s2:", key_length_s2)
Contributing
Contributions are welcome! If you find a bug or have suggestions for improvements, please open an issue or submit a pull request on GitHub.

License
This project is licensed under the MIT License.

Feel free to customize the documentation as needed, and don't forget to include the appropriate license file if you decide to use the MIT License.






