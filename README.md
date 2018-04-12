# Enable Thinkpad special keys on Debian 9.

mutemaster:	mutes the master channel

mutemic: 	mutes the microphone

volumedown: 	volume down

volumeup:	volume up

# Setting things up:

cp mutem* volume* /etc/acpi/events/

apt-get install amixer

systemctl restart acpid


