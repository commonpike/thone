# Thone - a terminal phone #


Thone is a suite of bash scripts to operate your daily phone: sms, call, etc.
The currently implemented commands are
sms, call, ppl and toggle. It does not yet handle dbus signals, such as
incoming calls, incoming messages or even outgoing calls; these should
still be handled by your default installation.

The first command is 'thone'. The other commands won't be available until you run 'thone'.

To learn the commands, try autocompletion, or `[command] help`, or read the [Documentation](Documentation.md).

### Install ###

Thone is in the shr-u feeds (thanks martin!), so if you're running shr, just type `opkg install thone`. Otherwise, the sources and ipkgs are in the download section.

To install from source, download the tarball and extract it in root. It will add files /usr/bin/thone-, /usr/share/thone/ , and a pixmap and desktop entry. Thats all. The first time you run thone, it sets up a /home/root/.thone dir.

### Dependencies ###

**Current dependencies - afaik:**

  * bash3 (opkg install bash)
  * python
  * python-dbus

**Future dependencies:**

  * signlaunchd (opkg install http://projects.openmoko.org/frs/download.php/724/siglaunchd_0.5.0-r0_armv4t.ipk)