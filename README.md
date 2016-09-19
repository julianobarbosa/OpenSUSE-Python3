# OpenSUSE-Python3
How to install Python3 in OpenSUSE from source
```console
zypper install --type pattern devel_C_C++ devel_python
zypper in libopenssl-devel libffi48-devel bluez-devel sqlite2-devel tk-devel valgrind-devel libexpat-devel sqlite3-devel readline-devel readline-devel-32bit libbz2-devel libexpat-devel libbz2-devel readline-devel sqlite3-devel
``` 
# Get Python3 Source
```console
cd /usr/src
wget -c https://www.python.org/ftp/python/3.5.2/Python-3.5.2.tar.xz
```
# Uncompress
```console
xz -d Python-3.5.2.tar.xz
tar xvf Python-3.5.2.tar
rm -rf Python-3.5.2.tar
```
# Configure Python3
```console
CXX="/usr/bin/g++"              \
./configure --prefix=/usr       \
            --enable-shared     \
            --with-system-expat \
            --with-system-ffi

```

