FreeBSD 9, 10, 11

Install dependencies:
```bash
pkg install cmake git ncurses boost-all log4cpp
```

Update linker paths:
```
/etc/rc.d/ldconfig restart
```


```bash
mkdir /usr/local/src
cd /usr/local/src
git clone https://github.com/FastVPSEestiOu/fastnetmon.git
cd fastnetmon
mkdir build
cd build
cmake ..
make
```

For netmap support you may need compile kernel manually with this [manual](BUILDING_FREEBSD_KERNEL_FOR_NETMAP.md).
