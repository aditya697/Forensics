# *SPIDERMAN*(E-challenge2)

We are given an image. By using exiftool we get a text in base64 in the comment.

By doing base64encoding we get the flag.``aW5jdGZ7M3gxZjcwMGxfMTVfbjFjZV8hX2d1M3NzX19fISEhIX0=``

*```FLAG:- inctf{3x1f700l_15_n1ce_!_gu3ss___!!!!}```*

# *QRCODE1*(SS_challenge2)

We are given a qr code. By using stegsolve by saving blue plane 0 image.

Then using ```zbarimg <filename>``` we get the flag.

*```FLAG:- VolgaCTF{5t3g0_m4tr3shk4_in_4cti0n}```*

# *QRCODE2*(Z-challenge2)

We are given a qr code. By using zbarimg we get the flag.

*```FLAG:- flag{QR_code_scanned}```*

# *ZEBRA*(s_challenge2)

We are given a image by using stegoveritas we can find the flag.

```stegoveritas <filename>``` by opening the results we can see the flag in trailing data.

*```FLAG:- inctf{5tr1ng5_4r3_us3ful_1_gu3s5}```*

# *COUNTER-STRIKE*(SH_challenge2)

We are given an image by using stegoveritas we can find the flag.

```stegoveritas <filename>``` by opening the results we can see flag in in base64 in the trailing data. By encoding the from we get the passsphrase ```Enimi3s_ah3ad```.

Now by using steghide tool we get the flag. ```steghide extract -sf <filename>```.

*```FLAG:-inctf{fr13ndly_f1re_is_s0met1m3s_d4ng3r0u5}```

# *REVERSE*

We are given text file which says reverse and we given one more file.

By using strings with the file along grep we can find the flag in reverse.

By using ```"}ss3ug_1_gn1sr3ver_t4_d00g_3ra_u0Y{ftcn"[::-1]``` we get flag by putting i in front.

*```FLAG:-inctf{Y0u_ar3_g00d_4t_rev3rs1ng_1_gu3ss}```*

