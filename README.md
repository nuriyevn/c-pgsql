# c-pgsql

#Installation

Installation steps for Red Hat based distros:
Mandatory:
yum install postgresql-devel
Optional:
export PATH=$PATH:/usr/pgsql-x.x/bin


Installation Steps for Debian Based distros:
Mandatory:
apt-get install libpq-dev

#Configuration

$ pg_config --includedir
/usr/include/postgresql
$ pg_config --libdir
/usr/lib

#Makefile
all:
        gcc testlibpq.c -o testlibpq.o -I/usr/include/pgsql92 -L/usr/lib64/pgsql92 -lpq







