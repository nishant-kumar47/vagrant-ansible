# vagrant-ansible

### Port forwarding: 
This has been implemented using firewalld forwarding
### Systemd file

In order to run the python script as a daemon, entry has to be made in systemd file. Version of Systemd insatlled(219) on machine didnt support Standard Output to a file on the machine.Hence provision to send the logs to syslog has been done. https://stackoverflow.com/questions/37585758/how-to-redirect-output-of-systemd-service-to-a-file

