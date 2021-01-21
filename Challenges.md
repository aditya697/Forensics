# ***THE OFFICE TROUBLE 1***

We are given a zip file in which there is jpeg file.
When try to open jpeg file we know that it is password encrypted.

So, By using ```fcrackzip``` tool we can find the password using dictionary attack

```fcrackzip -v -u -D -p rockyou.txt clients.zip```

We get the ```password:- perfectlypunk```

Using if we open the image we the flag

```FLAG:-inctfj{dw1ght_1s_cr4zy_bu7_awes0me}```

# ***SECURITY 101***

We are given zip file. Inside that we have 2 files a zip which is password protected 
and an image. 

Since the authors for both files are same by checking the author usind exiftool
and use it as the

```password:-R3DDIT_US3R``` for the the zip file we get the flag.

```FLAG:-inctfj{1ts_4ll_f1ne_tru5t_m3}```
