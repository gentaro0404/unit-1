# Quiz009

## Create a function that receives as input a stering and reaturns the string ciphered with shift 13.

```.py
PLAIN = "secret,-10"

KEY = 13

a = ""

for char in list(PLAIN):
    ASCII = ord(char)
    num = ASCII - 97
    num = (num + KEY) % 26
    ASCII = num + 97
    a += chr(ASCII)

print(a)
```
## Fig.1
![](quiz009.jpg)

## Flowchart:

