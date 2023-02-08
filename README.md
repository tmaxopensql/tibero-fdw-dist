Foregin Data Wrapper for Tibero
=============================== 

This PostgreSQL extension implements a Foreign Data Wrapper(FDW) for Tibero.

Supported OS
-------------
* Ubuntu20.04 <br>
* Centos7 , Centos8 <br>
* Redhat7 , Redhat8

Requirement 
------------

Shared libraries under < Supported OS system >/lib directories are essential for tibero_fdw operation.
Those libraries must be included in the LD_LIBRARY_PATH of the postgresql server process(Postmaster).

Installation 
--------------
  
To compile the Tibero foreign data wrapper, You need to ensure the `pg_config` executable is in your path when you run `make`. This executable is typically in your PostgreSQL installation's bin directory. 

Also you need PostgreSQL headers (if your PostgreSQL was installed with packages, install the development package).

1. Set LD_LIBRARY_PATH for Tibero client libraries.  
```
. ./setenv
```


2. Install Tibero foreign data wrapper.
```
make install 
```
