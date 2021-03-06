Configfile
----------

The config.ini is located in the direcory ``configs/`` and is used to
configure the MAD server in general. Stuff like database credentials,
websocket ports, MADmin, and runtype settings. Every parameter has its
own description and a default value. **If it doesn’t have a default
value, it’s a necessary parameter!**

.. note::  Make sure to leave a space after the colon if a value is needed. Example: ``example-setting-with: value``.

A different config-files can be included directly in processes by
``–config`` or ``-cf`` and path.


Mandatory parameters to run MAD:
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

+------------------+---------------------------------------------------------------------+
| Parameter        | Description                                                         |
+==================+=====================================================================+
| db_method        | The DB scheme to use. Either “monocle” or “rm” (without the quotes) |
+------------------+---------------------------------------------------------------------+
| dbip             | IP adress or hostname of the mysql server                           |
+------------------+---------------------------------------------------------------------+
| dbusername       | Username of database                                                |
+------------------+---------------------------------------------------------------------+
| dbpassword       | Password of database                                                |
+------------------+---------------------------------------------------------------------+
| dbname           | Name of the database                                                |
+------------------+---------------------------------------------------------------------+
| Runtype settings | Read more about them `here`_                                        |
+------------------+---------------------------------------------------------------------+

Recommended settings
^^^^^^^^^^^^^^^^^^^^
Those settings are not necessary but often used.

+------------------------+-----------------------+
| Parameter              | Description           |
+========================+=======================+
| with_madmin            | Start MAD with MADmin |
+------------------------+-----------------------+
| madmin_user            | Username for MADmin   |
+------------------------+-----------------------+
| madmin_password        | Password for MADmin   |
+------------------------+-----------------------+
| log_file_rotation_size | Enables logrotation   |
+------------------------+-----------------------+

.. _here: /scanning-modes/modes.md