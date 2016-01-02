# Thone - a Terminal Phone #

Thone is a terminal phone written in Bash3 and python for http://docs.freesmartphone.org based devices.

More precise, thone is a suite of bash scripts to operate your daily phone: sms, call, etc. It does not yet handle dbus signals, such as incoming calls, incoming messages or even outgoing calls; these should still be handled by your default software.

It requires
  * a linux based phone like http://www.openmoko.org
  * running on FSO and with the python/dbus library
  * bash3 installed


---

> Note: FSO has changed its interfaces and at least sms is not working anymore.  I'm working on it, as time permits ..

---


Running 'thone' starts a new (bash) shell and initializes Thone.
In that shell, you have additional commands like
```
> call +310652252252
> ppl add +31065225222 frank
> sms @frank answer your damn phone, i know youre there
> toggle sleep on
```
.. and autocompletion is your friend.

Thone is in the shr-u feeds (thanks martin!), so if you're running shr, just type `opkg install thone`. Otherwise, the sources and ipkgs are in the downloads section, instructions are [here](Introduction.md).

I'm using it on my Openmoko on SHR-U. It comes with a launcher icon for Enlightenment, which spawns Vala-terminal with 'thone jail' in it - so for example "sms read" looks like this:

![http://wiki.openmoko.org/images/thumb/8/82/Thone-example.jpg/180px-Thone-example.jpg](http://wiki.openmoko.org/images/thumb/8/82/Thone-example.jpg/180px-Thone-example.jpg)