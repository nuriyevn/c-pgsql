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

#Vim indentation
filetype plugin indent on
" show existing tab with 4 spaces width
set tabstop=4
" when indenting with '>', use 4 spaces width
set shiftwidth=4
" On pressing tab, insert 4 spaces
set expandtab





