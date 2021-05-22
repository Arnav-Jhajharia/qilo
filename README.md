# Qilo SSH

## Control multiple SSH servers at once

### How to use
* Download the github repository

* In the same directory as the main.py file, create a txt file such as info.txt

* In the info.txt, follow this format to specify the required information
```txt
192.168.1.13 22 user pass
```
Where 192.168.1.13 is the IP of the server, 22 is the port on which SSH is running, user is the username and pass is the username's password
<br>
You can add more IPs, ports, usernames and passwords but the corresponding information for each server should be on the same line separated by 1 space

* Save the file, mark main.py as an executable and run it as: ./main.py info.txt

* Enter the command as your input and the output for each server will be displayed

### Modules

* Ping: Pings IP addresses specified in the list. Can be used in the command input, by simply typing 'ping'

* OS Information: Displays the OS information of all servers in the list. Can be used in the command input, by simply typing 'os-info'

### Installation

```
git clone https://github.com/arav06/qilo-ssh/
cd qilo-ssh
pip install -r requirements.txt
chmod +x main.py
./main.py
```

### Requirements

* Python3

* Paramiko

### Updates

v1.1(Work in progress)
* Add support to use private keys 

* Endless connection to SSH server so that the program does not have to be run again to execute more commands

There will be more updates in the future
