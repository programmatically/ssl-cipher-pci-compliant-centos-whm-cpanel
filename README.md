# ssl-cipher-pci-compliant-centos-whm
This project is aimed at getting a PCI compliant SSL cipher server set-up for Centos/WHM that will still get an A+ on ssllabs.com

-V WHM 11.52.1

##Instructions

###Part 1

For the SSL Cipher Suite please read the instructions in the file



###Part 2

To upate post_virtualhost_global.conf and pre_virtualhost_global.conf navigate to...

Service Configuration > Apache Configuration > Include Editor

or 

SSH 

### nano /etc/apache2/conf.d/includes/pre_virtualhost_global.conf
### nano /etc/apache2/conf.d/includes/post_virtualhost_global.conf

after updating these files you must rebuild
###/scripts/rebuildhttpdconf && service httpd restart;

##Other


Please remember you must also look into editing your Cpanel Config, Exim Config and Mail Server Config SSL Ciphers for PCI compliance that is not covered here


###LEGAL

This content is a guide. No liability (ie. security holes, content loss or server downtime) or support, loss of finance, loss of visitors or users, etc can be applied for usage of this content what-so-ever so if you use this guide you are entirly responsible for anything that may or does go wrong.

