Vulnerability scanning is a crucial phase of a penetration test and having an updated vulnerability scanner in your security toolkit can often make a real difference by helping you discover overlooked vulnerable items. For this reason, we’ve manually packaged the latest and newly released OpenVAS 8.0 tool and libraries for Kali Linux. Although nothing major has changed in this release in terms of running the vulnerability scanner, we wanted to give a quick overview on how to get it up and running.

# apt-get update
# apt-get dist-upgrade

# apt-get install openvas
# openvas-setup
# openvas-start

To change the web login :

    openvasmd --create-user NEWUSER

It will automatically generate a password for the new user.

Use this new account to modify the admin password.

To remove the 'junk / false' account just enter

    openvasmd --delete-user=NEWUSER
    
or do so in the WebUI.

https://www.kali.org/penetration-testing/openvas-vulnerability-scanning/
http://serverfault.com/questions/563815/reset-admin-password-of-openvas