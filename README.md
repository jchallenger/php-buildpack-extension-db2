This is an extension for the Cloud Foundry PHP Buildpack:

This extension was orginally provided by the IBMDB buildpack. 
https://github.com/ibmdb/php-buildpack

I extracted the extension from the buildpack and modified it to support PHP 7.2+ using the new drivers (DB2 2.0.8 & PDO 1.3.8)
This extension automatically copies the correct versions of `ibm_db2.so` and `pdo_ibm.so` to the PHP Extensions directory, and IBM CLI Drivers to BP_DIR/ibm\_clidrivers.

**NOTE:L** php.ini is automatically edited by the script and `extension=ibm_db2.so` and `extension=pdo_ibm.so` are added, so you do not need to do anything additional to enable the extensions.
