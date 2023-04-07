# ROT13_Cipher

```py
def rot13(text):
    ciphered_text = ""
    for c in text:
        ascii_c = ord(c)
        if c.isalpha():
            if ord("a") <= ord(c) <= ord("m") or ord("A") <= ord(c) <= ord("M"):
                ascii_c = ord(c) + 13
            else:
                ascii_c = ord(c) - 13
        ciphered_text += chr(ascii_c)
    return ciphered_text


print("Now you are using ROT13 substitution cipher.")
text = input("Your text: ")
print(rot13(text))


```
