# Install OpenSSL Manually On Linux
## Downloading OpenSSL:

1. $ wget http://www.openssl.org/source/openssl-1.0.1g.tar.gz

Also, download the MD5 hash to verify the integrity of the downloaded file for just varifacation purpose. In the same folder where you have downloaded the OpenSSL file from the website :

1. $ wget http://www.openssl.org/source/openssl-1.0.1g.tar.gz.md5
2. $ md5sum openssl-1.0.1g.tar.gz
3. $ cat openssl-1.0.1g.tar.gz.md5

## Extract files from the downloaded package:
$ tar -xvzf openssl-1.0.1g.tar.gz

$ cd openssl-1.0.1g

## Configuration OpenSSL:

Run below command with optional condition to set prefix and directory where you want to copy files and folder.

$ ./config --prefix=/usr/local/openssl --openssldir=/usr/local/openssl

You can replace “/usr/local/openssl” with the directory path where you want to copy the files and folders. But make sure while doing this steps check for any error message on terminal.

## Compiling OpenSSL:
$ make

Note: check for any error message for verification purpose

## Installing OpenSSL:

$ sudo make install

Or without sudo,

$ make install

That’s it. OpenSSL has been successfully installed. You can run the version command to see if it worked or not as below :

$ /usr/local/openssl/bin/openssl version





