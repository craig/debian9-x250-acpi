# Enable Thinkpad special keys on Debian 9.

mutemaster:	mutes the master channel

mutemic: 	mutes the microphone

volumedown: 	volume down

volumeup:	volume up

# Testing

run acpi_listen, press Fn+F1, Fn+F2, Fn+F3, Fn+D4. Output should be similar:

button/mute MUTE 00000080 00000000 K

button/volumedown VOLDN 00000080 00000000 K

button/volumeup VOLUP 00000080 00000000 K

button/f20 F20 00000080 00000000 K



# Setting things up:

cp mutem* volume* /etc/acpi/events/

apt-get install amixer

systemctl restart acpid


