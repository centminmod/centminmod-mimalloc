Microsoft's [mimalloc](https://github.com/microsoft/mimalloc) general purpose memory allocator custom RPM build for Centmin Mod LEMP stacks's Nginx built binaries and EL7 CentOS 7 and EL8 Alma Linux/Rocky Linux 8. Optional alternative to Centmin Mod Nginx binaries which use jemalloc memory allocator by default.

# EL7

```
yum -q info mimalloc-custom
Installed Packages
Name        : mimalloc-custom
Arch        : x86_64
Version     : 2.0.6
Release     : 1.el7
Size        : 501 k
Repo        : installed
From repo   : /mimalloc-custom-2.0.6-1.el7.x86_64
Summary     : mimalloc-custom-2.0.6 for centminmod.com LEMP stack installs
URL         : https://centminmod.com
License     : unknown
Description : mimalloc-custom-2.0.6 for centminmod.com LEMP stacks
```
```
rpm -ql mimalloc-custom
/usr/local/nginx-dep/include/mimalloc-2.0/mimalloc-new-delete.h
/usr/local/nginx-dep/include/mimalloc-2.0/mimalloc-override.h
/usr/local/nginx-dep/include/mimalloc-2.0/mimalloc.h
/usr/local/nginx-dep/lib64/cmake/mimalloc-2.0/mimalloc-config-version.cmake
/usr/local/nginx-dep/lib64/cmake/mimalloc-2.0/mimalloc-config.cmake
/usr/local/nginx-dep/lib64/cmake/mimalloc-2.0/mimalloc-release.cmake
/usr/local/nginx-dep/lib64/cmake/mimalloc-2.0/mimalloc.cmake
/usr/local/nginx-dep/lib64/libmimalloc.so
/usr/local/nginx-dep/lib64/libmimalloc.so.2
/usr/local/nginx-dep/lib64/libmimalloc.so.2.0
/usr/local/nginx-dep/lib64/mimalloc-2.0/libmimalloc.a
/usr/local/nginx-dep/lib64/mimalloc-2.0/mimalloc.o
```

# EL8

```
yum -q info mimalloc-custom
Installed Packages
Name         : mimalloc-custom
Version      : 2.0.6
Release      : 1.el8
Architecture : x86_64
Size         : 587 k
Source       : mimalloc-custom-2.0.6-1.el8.src.rpm
Repository   : @System
From repo    : @commandline
Summary      : mimalloc-custom-2.0.6 for centminmod.com LEMP stack installs
URL          : https://centminmod.com
License      : unknown
Description  : mimalloc-custom-2.0.6 for centminmod.com LEMP stacks
```
```
rpm -ql mimalloc-custom
/usr/lib/.build-id
/usr/lib/.build-id/77
/usr/lib/.build-id/77/56d131498f5e8282f1a69ea14923229d14385c
/usr/local/nginx-dep/include/mimalloc-2.0/mimalloc-new-delete.h
/usr/local/nginx-dep/include/mimalloc-2.0/mimalloc-override.h
/usr/local/nginx-dep/include/mimalloc-2.0/mimalloc.h
/usr/local/nginx-dep/lib64/cmake/mimalloc-2.0/mimalloc-config-version.cmake
/usr/local/nginx-dep/lib64/cmake/mimalloc-2.0/mimalloc-config.cmake
/usr/local/nginx-dep/lib64/cmake/mimalloc-2.0/mimalloc-release.cmake
/usr/local/nginx-dep/lib64/cmake/mimalloc-2.0/mimalloc.cmake
/usr/local/nginx-dep/lib64/libmimalloc.so
/usr/local/nginx-dep/lib64/libmimalloc.so.2
/usr/local/nginx-dep/lib64/libmimalloc.so.2.0
/usr/local/nginx-dep/lib64/mimalloc-2.0/libmimalloc.a
/usr/local/nginx-dep/lib64/mimalloc-2.0/mimalloc.o
```

# Centmin Mod Nginx with systemd service files

For `/usr/lib/systemd/system/nginx.service` add `/etc/systemd/system/nginx.service.d/mimalloc.conf`

```
[Service]
Environment=LD_PRELOAD=/usr/local/nginx-dep/lib64/libmimalloc.so.2
```
```
systemctl daemon-reload
systemctl restart nginx
```
```
lsof | grep libmimalloc.so | head -n2
nginx      2828             root  mem       REG                9,1     135648     760804 /usr/local/nginx-dep/lib64/libmimalloc.so.2.0
nginx      2829            nginx  mem       REG                9,1     135648     760804 /usr/local/nginx-dep/lib64/libmimalloc.so.2.0
```

Centmin Mod Nginx with mimalloc 2.0.6

```
ps aufxw | grep 'nginx:' | grep -v grep
root      2828  0.0  0.5 540440 173108 ?       Ss   11:20   0:00 nginx: master process /usr/local/sbin/nginx -c /usr/local/nginx/conf/nginx.conf
nginx     2829  0.0  1.0 851796 342488 ?       S<l  11:20   0:00  \_ nginx: worker process
nginx     2830  0.0  1.0 851796 342488 ?       S<l  11:20   0:00  \_ nginx: worker process
nginx     2831  0.0  1.0 851796 342488 ?       S<l  11:20   0:00  \_ nginx: worker process
nginx     2832  0.0  1.0 851796 342488 ?       S<l  11:20   0:00  \_ nginx: worker process
nginx     2833  0.0  1.0 851796 342488 ?       S<l  11:20   0:00  \_ nginx: worker process
nginx     2834  0.0  1.0 851796 343672 ?       S<l  11:20   0:00  \_ nginx: worker process
nginx     2835  0.0  1.0 851796 342488 ?       S<l  11:20   0:00  \_ nginx: worker process
nginx     2836  0.0  1.0 851796 342956 ?       S<l  11:20   0:00  \_ nginx: worker process
```

Compared to Centmin Mod Nginx with jemalloc 5.3.0

```
ps aufxw | grep 'nginx:' | grep -v grep
root      4195  0.2  0.5 452244 171960 ?       Ss   11:24   0:00 nginx: master process /usr/local/sbin/nginx -c /usr/local/nginx/conf/nginx.conf
nginx     4196  0.4  1.0 743944 341344 ?       S<l  11:24   0:00  \_ nginx: worker process
nginx     4197  0.4  1.0 743944 341344 ?       S<l  11:24   0:00  \_ nginx: worker process
nginx     4198  0.4  1.0 743944 341344 ?       S<l  11:24   0:00  \_ nginx: worker process
nginx     4199  0.4  1.0 743944 341344 ?       S<l  11:24   0:00  \_ nginx: worker process
nginx     4200  0.4  1.0 743944 341824 ?       S<l  11:24   0:00  \_ nginx: worker process
nginx     4201  0.4  1.0 743944 341344 ?       S<l  11:24   0:00  \_ nginx: worker process
nginx     4202  0.3  1.0 743944 341344 ?       S<l  11:24   0:00  \_ nginx: worker process
nginx     4203  0.3  1.0 743944 341344 ?       S<l  11:24   0:00  \_ nginx: worker process
```

Compared to Centmin Mod Nginx with jemalloc 3.6.0 default

```
ps aufxw | grep 'nginx:' | grep -v grep
root     22715  0.1  0.5 437864 171680 ?       Ss   22:30   0:00 nginx: master process /usr/local/sbin/nginx -c /usr/local/nginx/conf/nginx.conf
nginx    22722  0.3  1.0 745128 341044 ?       S<l  22:30   0:00  \_ nginx: worker process
nginx    22724  0.2  1.0 745128 341044 ?       S<l  22:30   0:00  \_ nginx: worker process
nginx    22728  0.2  1.0 745128 341044 ?       S<l  22:30   0:00  \_ nginx: worker process
nginx    22730  0.3  1.0 745128 341044 ?       S<l  22:30   0:00  \_ nginx: worker process
nginx    22735  0.3  1.0 745128 341044 ?       S<l  22:30   0:00  \_ nginx: worker process
nginx    22737  0.2  1.0 745128 341044 ?       S<l  22:30   0:00  \_ nginx: worker process
nginx    22740  0.2  1.0 745128 341044 ?       S<l  22:30   0:00  \_ nginx: worker process
nginx    22759  0.2  1.0 745128 341044 ?       S<l  22:30   0:00  \_ nginx: worker process
```

# Other Usage

mimalloc is a drop-in replacement for malloc and can be used in other programs besides Centmin Mod Nginx without code changes, for example, on dynamically linked ELF-based systems (Linux, BSD, etc.) you can use it as:

```
LD_PRELOAD=/usr/local/nginx-dep/lib64/libmimalloc.so.2 myprogram
```