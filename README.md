# Droid Module: droid/hostname

Change the host name. For more information on Droid, please see
[droidphp.com](http://droidphp.com).

The steps involved are:-

1. Write the new host name into the templated shell script and copy it to the
   host.
2. Execute the shell script on the host.


## Assumptions

1. The platform is Debian-based.
2. The host name configuration of the host is in a consistent state.  The shell
   script will either make *all* of the required changes or *none* of them,
   depending on whether the host name is different from that proposed.


## Limitations

1. The shell script will simply replace, in `/etc/hosts`, all instances of the
   existing name, wherever they might occur, with the proposed name.


## Information required by the module

None.


## Optional information

None.
