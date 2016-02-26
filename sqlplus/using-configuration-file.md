# Using configuration file
SQLPLUS accept 2 kinds of configuration file that is loaded automatically when you start it.

Whenever SQL*PLUS starts up, it looks for a file named `glogin.sql` under the directory `$ORACLE_HOME/sqlplus/admin`. After reading `glogin.sql` SQLPLUS looks for a file named `login.sql` under the directory that enviroment variable `SQLPATH` points (normally the directory where SQLPLUS is started) to and reads it and executes its.
