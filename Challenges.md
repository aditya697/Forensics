# ***THE OFFICE TROUBLE 1***

We are given a zip file in which there is jpeg file.
When try to open jpeg file we know that it is password encrypted.

So, By using ```fcrackzip``` tool we can find the password using dictionary attack

```fcrackzip -v -u -D -p rockyou.txt clients.zip```

We get the ```password:- 
