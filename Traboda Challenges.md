# ***SNOW SNOW***

We are given a text. The flag is hidden in the spaces.
Using stegsnow tool we can find what is hidden.

```stegsnow -C <filename>```

We get ```ntio{eP1B35x4K3_aB3O0_q5_K00t}```
By rotating the bit by 18 we get the flag coz the flag starts with *f*
 we can guees can that it is rotated by 18.
 
 ```FLAG:-flag{wH1T35p4C3_sT3G0_i5_C00l}```
 
 # ***SNOW MAN***
 
 We are give a text. The text says password is ``thisiseasy``
 Using stegsnow tool we can find hidden data in text with password.
 
 ```stegsnow -C -p "thisiseasy" <filename>```
 
 We get ``aW5jdGZqe2g0aDRfc3QzZ3NuMHdfaTVfYzAwMDAwMDAxfQ==``
 By doing base64 we get the flag.
 
 ```FLAG:-inctfj{h4h4_st3gsn0w_i5_c00000001}```
 
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
To extract data from ``.PNG`` file we can use stegsolve tool.
By using ``java -jar stegsolve.jar`` being in the `bin` directory.
When we open the file using stegsolve and when we see different photos by clicking next.
Or we can use this image analyser ``https://compress-or-die.com/analyze``.
We get flag using this stegsolve tool.


```FLAG:-inctfj{th3_fl4g_wa5_liter4lly_ins1de_4_m3me}```

# ***DETAILED VEIW***
 We are given a .PNG file.
 
 If we do ``strings <filename>`` we get a link ``https://pastebin.com/KudUCfTC``in the ending.
 
 Opening that we see a text.By doing BASE64 decoding we get the flag.
 ```
>>> from base64 import b64decode
>>> b64decode(b'ZmxhZ3tNMTVzSTBOX2FDYzBNUEwxNWgzRH0=')
b'flag{M15sI0N_aCc0MPL15h3D}'
``` 
 ```FLAG:-flag{M15sI0N_aCc0MPL15h3D}```

# ***BACK TO SAN ANDREAS***

We a given a ``.jpg`` file.Using jsteg tool We can find the flag.

```jsteg reveal <filename.jpg> <output_filename>``` If we open the output file we can see the flag.

```FLAG:-inctfj{gr0ve_5treet_f0r_l1fe}```

# ***MY_FIRST_STEGNOGRAPHY***

We are given 2 ``.jpg`` files. We can get the flag using ``steghide``.

For the first file there is no passphrase. So by using ``steghide extract -sf <filename>`` We get the password for the next file.
We get passphrase as ``d4rk_s1d3``

By using ``steghide -sf <filename>`` and giving passphrase that we got earlier we get the flag.

```FLAG:-inctfj{w3_4r3_pl4nt1ng_4_b0mb}```

# ***CON ON CAT***

We are given a ``.PNG``. By using ``pngcheck -v <filename>``

We get that after IEND data is there.Using ``foremost -v <filename>`` we can extract the file.

We get a file which has 4 images in that we will have flag in 1 image.

```FLAG:-inctfj{y0u_c4nt_s33_m3!!}```

# ***THE OFFICE TROUBLE 2***

We a given ``pdf file`` which is password protected.

By using ``PDFcrack`` ```pdfcrack -f <filename> -w <wordlist>``` we cam find the ``password = fear420``

```FLAG:-inctfj{ass1stant_t0_th3_regi0nal_man4ger}```

# ***HIDDEN DATA***

We are given a zip file which is corrupted. By changing the header of the zip file.

By unzipping it we get the flag.

*```FLAG:-inctfj{GR3aT_m155i0n_4Cc0mpL15h3D}```*

# ***CORRUPTED FILE***

We are given a zip file which is corrupted. By changing the header of the zip file.

By unzipping it we get a base64 encoded string by decoding it we get the flag.

*```FLAG:-flag{9e360084196a092a15c5c44b54934bfc}```*

# ***CRACK PDF***

We are given pdf file, which is password protected.

We can crack the password using pdfcrack dictionary attack ```diosayudameenelesut```.

After getting the password when we open the and seacrh for the word flag we get the flag.

*```FLAG:-flag{1ae06a29a7abd6c07dba8976698f756b987f734d```*
