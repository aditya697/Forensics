# ***SNOW SNOW***

We are given a text. The flag is hidden in the spaces.
Using stegsnow tool we can find what is hidden.

```stegsnow -C <filename>```

We get ```ntio{eP1B35x4K3_aB3O0_q5_K00t}```
By rotating the bit by 18 we get the flag coz the flag starts with *f*
 we can guees can that it is rotated by 18.
 
 ```FLAG:-flag{wH1T35p4C3_sT3G0_i5_C00l}```
 
 # ***10111001***
 
  We are given `.PNG`. We should use zsteg tool.
  
  Then we get ``` "Here is your flag : NFXGG5DGNJ5TI3K7ORUDGX2MGNAVG5C7GVUUO3RRMYYWGNDOKRPWEVKUL4YV6YZUJZPXI4RQOVBEYM27LEYHKXZUL5WDAVD5"```
  
  By using BASE32 decoding, we get the flag.
  
  ```FLAG:-inctfj{4m_th3_L3ASt_5iGn1f1c4nT_bUT_1_c4N_tr0uBL3_Y0u_4_l0T}```
  
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

# ***YOU CAN'T SEE ME***

We are given a .png file. If we try to open the image.
It won't open because the file is corrupted.

By using ```hexedit```we edit the file format to `.PNG`.

By clearing the remaining ``chunks`` we can open the image and find the flag.

```FLAG:-inctfj{WH4t_ar3_pNgCHUnkS?}```

# ***JAY-CHOT***
 We are given a `.jpg` file. 
 But the file format is not correct by editing 
 the file format. 
 
 We get the flag if we open the image.
 
 ```FLAG:-flag{a4aa04741a8d3a952a7ec88457991b97}```
 
# ***MAGIC IN DIGITS***

We are given a .png file. If we try to open the image.
It won't open because the file is corrupted.

By using ```hexedit```we edit the file format to `.PNG`.

By clearing the remaining ``chunks`` we can open the image and find the flag.

```FLAG:-flag{Chunks_4r3_1mpor74an7_f0r_1mage5}```

# ***ALWAYS HAS BEEN***

We are given a ``.PNG`` file. It has data inside it.
To extract data from ``.PNG`` file we can use zsteg tool.
Or we can use this image analyser ``https://compress-or-die.com/analyze``.
We get flag using this zsteg tool.

```FLAG:-inctfj{th3_fl4g_wa5_liter4lly_ins1de_4_m3me}```

# ***DETAILED VEIW***
 We are given a .PNG file.
 
 If we do ``string <filename>`` we get a link ``https://pastebin.com/KudUCfTC``in the ending.
 
 Opening that we see a text.By doing BASE64 decoding we get the flag.
 ```
>>> from base64 import b64decode
>>> b64decode(b'ZmxhZ3tNMTVzSTBOX2FDYzBNUEwxNWgzRH0=')
b'flag{M15sI0N_aCc0MPL15h3D}'
``` 
 ```FLAG:-flag{M15sI0N_aCc0MPL15h3D}```
