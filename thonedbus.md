# Thone-dbus #

Thone-dbus is written in python. It's a rewrite of mdbus (the 'mickey dbus'), with some custom hardcoded logic for thone.



example of some prewritten thone-dbus calls:
```
 > thone-dbus update-sms
 > thone-dbus update-call
 > thone-dbus update-ppl
```

example of a raw thone-dbus call:
```
 >thone-dbus org.freesmartphone.ogsmd \	# busname
 	/org/freesmartphone/GSM/Device \# objname
 	org.freesmartphone.GSM.SIM \	# ifacename
	RetrieveMessagebook \		# methodname
 	all				# parameters
```

For the api on raw calls, check http://docs.freesmartphone.org