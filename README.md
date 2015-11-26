# ssl-cipher-pci-compliant-centos-whm
This project is aimed at getting a PCI compliant SSL cipher server set-up for Centos/WHM that will still get an A+ on ssllabs.com


To upate post_virtualhost_global.conf and pre_virtualhost_global.conf navigate to...

Service Configuration > Apache Configuration > Include Editor

or 

SSH 

### nano /etc/apache2/conf.d/includes/pre_virtualhost_global.conf
### nano /etc/apache2/conf.d/includes/post_virtualhost_global.conf

after updating these files you must rebuild
###/scripts/rebuildhttpdconf && service httpd restart;



Please remember you must also look into editing your Cpanel Config, Exim Config and Mail Server Config SSL Ciphers for PCI compliance that is not covered here

