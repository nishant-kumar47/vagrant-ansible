# vagrant-ansible

### Port forwarding: 
I have used my personal laptop which is a windows 10 machine. There seems to be a issue with port forwarding from windows machine to 
linux box. however app can be accessed on : curl http://10.10.10.20:5000 from host machine. Port forwarding from 80-5000 is not working due to host issues.This can be due to virtual box guest addition too. Please run "vagrant plugin install vagrant-vbguest"
### Systemd file

In order to run the python script as a daemon, entry has to be made in systemd file. Version of Systemd insatlled(219) on machine didnt support Standard Output to a file on the machine.Hence provision to send the logs to syslog has been done. https://stackoverflow.com/questions/37585758/how-to-redirect-output-of-systemd-service-to-a-file

