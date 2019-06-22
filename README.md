This is an extension for the Cloud Foundry PHP Buildpack:
https://github.com/cloudfoundry/php-buildpack

This extension was orginally provided by the IBMDB buildpack. 
https://github.com/ibmdb/php-buildpack

I extracted the extension from the buildpack and modified it to support PHP 7.2+ using the new driver (DB2 2.0.8)
This extension automatically copies the correct version of `ibm_db2.so` to the PHP Extensions directory, and IBM CLI Drivers to `BP_DIR/ibm/_clidrivers`. 
`php.ini` is automatically edited by the script and `extension=ibm_db2.so` is added, so you do not need to do anything additional to enable the extension.
