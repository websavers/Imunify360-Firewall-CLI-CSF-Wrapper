# Imunify360 Firewall CLI CSF Wrapper
 Imunify360's CLI tools cover a lot of functionality, but they're not very concise. This wrapper script solves that problem by making IP bans, searches, ban removals closer to CSF's simpler syntax

## Installation Instructions
 - Ensure you have Imunify360 installed
 - Via SSH, as root, run: 

 ```
 curl -o /usr/local/bin/imu https://raw.githubusercontent.com/websavers/Imunify360-Firewall-CLI-CSF-Wrapper/master/imu
 chmod +x /usr/local/bin/imu
 ln -s /usr/local/bin/imu /usr/bin/imu
 ```
The symlink ensures imu is available as a command by being in the $PATH var.

## Usage
`imu -d [ip] [description]` -- denies an IP address
`imu -dr [ip]` -- remove IP from the deny list
`imu -g [ip]` -- greps/searches the IP bans for the specified IP
