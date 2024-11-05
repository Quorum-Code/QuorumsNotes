#linux #ip #domain #hostname #ip-resolution

# Adding an IP to Known Hosts 
## Editing Hosts File
`sudo vim /etc/hosts`

Opens the Vim text editor to manipulate the hosts text file, required super user permissions. 
## Append IP and Domain
`[IPv4] [HOSTNAME]`

Add an entry as the above, where IPv4 is like `192.168.39.79` and Hostname is like `hello.example.com`. 
### Appending Multiple Hostnames to a Single IP
It is possible to direct multiple hostnames to a single IP by appending new Hostnames to the end of the row, where each Hostname is separated by a space.