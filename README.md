
About
=====
**FiSH/Mircryption clone for HexChat in 100% Python**

* Encrypt/decrypt private conversations
* Encrypt/decrypt channel conversations
* Choose between ECB and CBC
* Automatic DH key exchange (private conversations only)

Installation
============
1. Put [fishcrypt.py](https://raw.githubusercontent.com/fladd/py-fishcrypt/master/fishcrypt.py) into HexChat addons folder:
  * Linux/OS X: ``~/.config/hexchat/addons/``
  * Windows: ``%APPDATA%\HexChat\addons\``
2. Start HexChat
3. Issue the command: ``/FISHSETUP``

*FiSHLim will be disabled when fishcrypt.py is loaded!*

Usage
=====

Commands
--------
```
SETKEY          set a new key for a nick or channel /SETKEY <nick>/#chan [new_key]
KEYX            exchange a new pub key, /KEYX <nick>
KEY             list key of a nick or channel or all (\*), /KEY [nick/#chan/\*]
DELKEY          remove key, /DELKEY <nick>/#chan/*

ME+             send crypted CTCP ACTION
MSG+            send crypted msg regardless of /ENCRYPT setting
NOTICE+         send crypted notice regardless of /ENCRYPT setting

CBCMODE         set or shows cbc mode for (current) channel/nick , /CBCMODE [<nick>] <0|1>
PROTECTKEY      sets or shows key protection mode for (current) nick, /PROTECTKEY [<nick>] <0|1>
ENCRYPT         set or shows encryption on for (current) channel/nick , /ENCRYPT [<nick>] <0|1>
PRNCRYPT        print msg encrpyted localy , /PRNCRYPT <msg>
PRNDECRYPT      print msg decrpyted localy , /PRNDECRYPT <msg>
DBPASS          set/change the passphrase for the Key Storage
DBLOAD          loads the Key Storage

SET fishcrypt   show additional fishcrypt settings
SET <SETTING>   set additional fishcrypt setting <SETTING>

HELP fishcrypt  show fishcrypt help
FISHUPDATE      Update fishcript
```

Licence
=======

fishcrypt.py
------------
Copyright 2011 Nam T. Nguyen (http://www.vithon.org/forum/Thread/show/54)

Released under the BSD license

rewritten by trubo/segfault for irc.prooops.eu #py-fishcrypt trubo00@gmail.com

fixed for HexChat by fladd <fladd@fladd.de>

irccrypt module is copyright 2009 Bjorn Edstrom ( http://www.bjrn.se/ircsrp )
with modification from Nam T. Nguyen and trubo

pyBlowfish.py
-------------
Copyright 2002 Michael Gilfix <mgilfix@eecs.tufts.edu>

Released under GPL or Artistic Licence

modified by trubo
