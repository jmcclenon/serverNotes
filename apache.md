## Install Apache Server on Ubuntu

1. Install Apache using the following:

	sudo apt-get install lamp-server^ (__make sure you include the ^ at the end__)
	
2. When done, you will have a functional Apache server installed on your machine. You should be able to use a browser, go to the IP address of the server. If you see the Apache startup page, all is well. If you don't see that page, try the installation again.

3. After installation, you may want to get the latest version of Apache 2, and update your repository information, so that you stay up-to-date with version updates. To do this, you will need to use a PPA. Type the following into your terminal (assuming Linux):

	sudo add-apt-repository ppa:ondrej/apache2
	sudo apt-get update
	sudo apt-get upgrade
	sudo apt-get dist-upgrade
	
4. When done, check your Apache version number. You can use php.info to establish this information (see below).

	<?php
	phpinfo();
	?>

The PHP code shown above, when run, will display a great deal of information about your Apache2/PHP platform. That will include the current Apache2 version number. It is probably a good idea to delete phpinfo.php when you're done using it. Too much information.

5. You may want to restart Apache2:

	service apache2 restart
	
For more information about the Apache2 PPA, check out this website:

https://launchpad.net/~ondrej/+archive/ubuntu/apache2
