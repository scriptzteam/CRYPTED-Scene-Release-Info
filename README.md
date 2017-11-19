# [CRYPTED] Scene-Release-Info
Get scene release info - **.nfo|.sfv|.jpg|.diz|.releaseinfo**, they are stored only for **14 days** so be quick!

**Video instruction - https://i.imgur.com/HA1Aibf.gifv**

You can also now get our generated files too for rar(s)/zip(s) of scene releases -> https://scriptz-team.info/index.php?post=4, they have extension called **.releaseinfo**

Everything is pgp/gpg crypted with key inside filename.crypt file

filename.crypt format:
```
https://transfer.sh/SOMETOKEN/SOMEKEY
:KEY:SOMEKEY
```

Main site:
```
https://archive.predb.pw/
```

Example:
```
https://archive.predb.pw/2017/11/19/aventyr.i.tid.och.rum.s01e12.swedish.720p.web.h264-swewr.sfv.crypt
```

Example output:
```
https://transfer.sh/RWY5R/VeOx8qvWNaFoAi3BO4tsUW3nblfaDp
:KEY:VeOx8qvWNaFoAi3BO4tsUW3nblfaDp
```

If you download the file and open it you will get this:
```
-----BEGIN PGP MESSAGE-----
Version: GnuPG v1

jA0EBwMCrWB0iDzdo4Rg0q4B3fL9fvUU6VXWx3nJn+QaLmH9ARj5TwvZeCYwZD8b
RTI6OyAVaLxLI38FRCnArKJ6W6os8JsBwMSGU0BfGEY1r2n6snUSRRMgGh0BHRoA
nzFMhCvTjzoPGH3+yZwMSSdKH3lU0qqGwuCF9SWsdAyW+d0WSlMd/3xI3P1/ZbH3
bLTKTG/hdlXbsdLvqlwX/skKGioIeFM9bNN4dhFiui3yuAtyEx0+osCRT/KlmBY=
=OATn
-----END PGP MESSAGE-----
```

So you will need to decrypt it, but hey its easy ;)

How to decrypt our example:
```
curl https://transfer.sh/RWY5R/VeOx8qvWNaFoAi3BO4tsUW3nblfaDp|gpg -o- > /tmp/decoded.txt
```

After you put this into your console it will ask for password to decrypt it.
Every file have own passwod.
The password is reversed text from **:KEY:VeOx8qvWNaFoAi3BO4tsUW3nblfaDp** and string **:KEY:** is removed also, so for our example the right password is **pDaflbn3WUst4OB3iAoFaNWvq8xOeV**, after that if you do cat /tmp/decoded.txt you can see decrypted file.

Regardz!
