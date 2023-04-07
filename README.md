# ROT13_Cipher

def rot13(text): <br>
    ciphered_text = ""<br>
    for c in text:<br>
        ascii_c = ord(c)<br>
        if c.isalpha():<br>
            if ord("a") <= ord(c) <= ord("m") or ord("A") <= ord(c) <= ord("M"):<br>
                ascii_c = ord(c) + 13<br>
            else:<br>
                ascii_c = ord(c) - 13<br>
        ciphered_text += chr(ascii_c)<br>
    return ciphered_text<br>
<br>
<br>
print("Now you are using ROT13 substitution cipher.")<br>
text = input("Your text: ")<br>
print(rot13(text))
