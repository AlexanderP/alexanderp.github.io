**notesalexp.org** - Unofficial repository for **Debian GNU/Linux** and **Ubuntu**. 
You can find the packages of this repository following this [link](http://notesalexp.org/packages/).

**Instructions**

_1. Open a terminal and install apt-transport-https_

	sudo apt-get install apt-transport-https

_2. Open /etc/apt/sources.list_

Add this line for **Wheezy**: `deb https://notesalexp.org/debian/wheezy/ wheezy main`  
Add this line for **Jessie**: `deb https://notesalexp.org/debian/jessie/ jessie main`  
Add this line for **Stretch**: `deb https://notesalexp.org/debian/stretch/ stretch main`  
Add this line for **Buster**: `deb https://notesalexp.org/debian/buster/ buster main`  
Add this line for **Sid**: `deb https://notesalexp.org/debian/sid/ sid main`  
Add this line for **Precise**: `deb https://notesalexp.org/debian/precise/ precise main`  
Add this line for **Trusty**: `deb https://notesalexp.org/debian/trusty/ trusty main`  
Add this line for **Xenial**: `deb https://notesalexp.org/debian/xenial/ xenial main`  
Add this line for **Bionic**: `deb https://notesalexp.org/debian/bionic/ bionic main`  
Add this line for **Cosmic**: `deb https://notesalexp.org/debian/cosmic/ cosmic main`  

Save and close sources.list

_3.Fetch and install the GnuPG key_

	sudo apt-get update -oAcquire::AllowInsecureRepositories=true
	sudo apt-get install notesalexp-keyring -oAcquire::AllowInsecureRepositories=true
	sudo apt-get update

or

	wget -O - https://notesalexp.org/debian/alexp_key.asc | sudo apt-key add -
	sudo apt-get update

_4. Enjoy_

	sudo apt-get install package
**Warning**: Need to update the gpg-key.(2018-09-13)  
**Warning**: Some packages for Debian GNU/Linux require http://www.deb-multimedia.org/ repository to be connected.

**[Support the project on Patreon.](https://www.patreon.com/notesalexp)**
