no-ip-updater
=============

Python module to update No-IP server


Installing
----------

	$ python setup.py install
	

Usage
-----

	import no_ip_updater
	no_ip_updater.update(username, password, host, ip)
	
### Command line ###
To update from command line:

	$ update-no-ip -u user -p pass -host ahost otherhost -ip myip
	
You can define in the script, a default user name, host, and even a password (not recommended).
If not defined, the password will be prompted.
If the IP is not passed on the command line, it will use the current IP.

---

[Note about some alternatives](https://github.com/steinerkelvin/no-ip-updater/issues/2#issuecomment-2012397753),
as No-IP requires periodic manual action to keep your domains. (We are not going to implement auto-renewal here).
