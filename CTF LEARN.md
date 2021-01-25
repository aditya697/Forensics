# *Binwalk*

We are given a .PNG file. By using pngcheck -v <filename>
we know that the file has extended data.

To extract data use foremost -v <filename>

```FLAG:-ABCTF{B1nw4lk_is_us3ful}```

# *WOW.. So meta*

We are given .jpg file.
By using exiftool we can find the flag.

```FLAG:-flag{EEe_x_I_FFf}```
 
 # *Rubber duck*
 
 We are given a .jpg file. 
 By using exiftool we get the flag.
 
 ```FLAG:-CTFlearn{ILoveJakarta}```

# *Snow Board*

We are given image. If we use strings <filename>.
We can see a flag but that is not the correct flag.

The bellow it must be base64decoded to get the flag.

```FLAG:-CTFlearn{SkiBanff}```

# *PikesPeak*

We are given a .jpg file. By using strings<filename>.
We get many flag trying out apropriate ones one will be correct.

```FLAG:-CTFlearn{Gandalf}```

# *ChalkBoard*

We are given a .jpg file. By using strings<filename>.We get
```
 CTFlearn{I_Like_Math_x_y}
where x and y are the solution to these equations:
3x + 5y = 31
7x + 9y = 59
```
By solving equations we get x=2 y=5
 
```FLAG:-CTFlearn{I_Like_Math_2_5}```
