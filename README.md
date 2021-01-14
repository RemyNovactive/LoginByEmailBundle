EabLoginByEmailBundle
=====================

A Symfony bundle enabling users to login to eZ Publish using either username or email address.

Summary
-------

This bundle enables users to login to eZ Publish using their email address in addition
to their username (this functionality was removed from eZ Publish in version 5.3).
To do so, we override eZ Publish's `UserProvider` and `AuthenticationProvider`.


FORK
----

forked from eab-dev/LoginByEmailBundle

*Why ?*

To make it compatible with eZ 2.5

Acknowledgements
----------------

Thanks to [silver.solutions](http://silversolutions.de) product development team
for [providing the information](http://blog.silversolutions.de/2014/07/ezpublish/extend-ez-5-3-login-email)
on how to do this.

Installation
------------

Edit `ezpublish\EzPublishKernel.php` and add the following to the `$bundles` array in the `registerBundles()` function:

```
new Eab\LoginByEmailBundle\EabLoginByEmailBundle(),
```
