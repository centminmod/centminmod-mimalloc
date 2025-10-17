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
/usr/local/nginx-dep/include/mimalloc-new-delete.h
/usr/local/nginx-dep/include/mimalloc-override.h
/usr/local/nginx-dep/include/mimalloc.h
/usr/local/nginx-dep/lib/cmake/mimalloc/mimalloc-config-version.cmake
/usr/local/nginx-dep/lib/cmake/mimalloc/mimalloc-config.cmake
/usr/local/nginx-dep/lib/cmake/mimalloc/mimalloc-release.cmake
/usr/local/nginx-dep/lib/cmake/mimalloc/mimalloc.cmake
/usr/local/nginx-dep/lib/libmimalloc.a
/usr/local/nginx-dep/lib/libmimalloc.so
/usr/local/nginx-dep/lib/libmimalloc.so.2
/usr/local/nginx-dep/lib/libmimalloc.so.2.0
/usr/local/nginx-dep/lib/mimalloc.o
```

# EL8

```
rpm -qpi mimalloc-custom-2.2.4-1.el8.x86_64.rpm
Name        : mimalloc-custom
Version     : 2.2.4
Release     : 1.el8
Architecture: x86_64
Install Date: (not installed)
Group       : default
Size        : 812195
License     : unknown
Signature   : (none)
Source RPM  : mimalloc-custom-2.2.4-1.el8.src.rpm
Build Date  : Fri 17 Oct 2025 06:01:21 CDT
Build Host  : build.domain.com
Relocations : / 
Packager    : <centminmod.com>
Vendor      : none
URL         : https://centminmod.com
Summary     : mimalloc-custom-2.2.4 for centminmod.com LEMP stack installs
Description :
```
```
rpm -qpl mimalloc-custom-2.2.4-1.el8.x86_64.rpm
/usr/local/nginx-dep/include/mimalloc-new-delete.h
/usr/local/nginx-dep/include/mimalloc-override.h
/usr/local/nginx-dep/include/mimalloc-stats.h
/usr/local/nginx-dep/include/mimalloc.h
/usr/local/nginx-dep/lib/cmake/mimalloc/mimalloc-config-version.cmake
/usr/local/nginx-dep/lib/cmake/mimalloc/mimalloc-config.cmake
/usr/local/nginx-dep/lib/cmake/mimalloc/mimalloc-release.cmake
/usr/local/nginx-dep/lib/cmake/mimalloc/mimalloc.cmake
/usr/local/nginx-dep/lib/libmimalloc.a
/usr/local/nginx-dep/lib/libmimalloc.so
/usr/local/nginx-dep/lib/libmimalloc.so.2
/usr/local/nginx-dep/lib/libmimalloc.so.2.2
/usr/local/nginx-dep/lib/mimalloc.o
/usr/local/nginx-dep/lib/pkgconfig/mimalloc.pc
```

# EL9

```
rpm -qpi mimalloc-2.2.4/mimalloc-custom-2.2.4-1.el9.x86_64.rpm
Name        : mimalloc-custom
Version     : 2.2.4
Release     : 1.el9
Architecture: x86_64
Install Date: (not installed)
Group       : default
Size        : 812695
License     : unknown
Signature   : (none)
Source RPM  : mimalloc-custom-2.2.4-1.el9.src.rpm
Build Date  : Fri 17 Oct 2025 03:38:19 AM PDT
Build Host  : build.domain.com
Relocations : / 
Packager    : <centminmod.com>
Vendor      : none
URL         : https://centminmod.com
Summary     : mimalloc-custom-2.2.4 for centminmod.com LEMP stack installs
Description :
```

```
rpm -qpl mimalloc-2.2.4/mimalloc-custom-2.2.4-1.el9.x86_64.rpm
/usr/local/nginx-dep/include/mimalloc-new-delete.h
/usr/local/nginx-dep/include/mimalloc-override.h
/usr/local/nginx-dep/include/mimalloc-stats.h
/usr/local/nginx-dep/include/mimalloc.h
/usr/local/nginx-dep/lib/cmake/mimalloc/mimalloc-config-version.cmake
/usr/local/nginx-dep/lib/cmake/mimalloc/mimalloc-config.cmake
/usr/local/nginx-dep/lib/cmake/mimalloc/mimalloc-release.cmake
/usr/local/nginx-dep/lib/cmake/mimalloc/mimalloc.cmake
/usr/local/nginx-dep/lib/libmimalloc.a
/usr/local/nginx-dep/lib/libmimalloc.so
/usr/local/nginx-dep/lib/libmimalloc.so.2
/usr/local/nginx-dep/lib/libmimalloc.so.2.2
/usr/local/nginx-dep/lib/mimalloc.o
/usr/local/nginx-dep/lib/pkgconfig/mimalloc.pc
```

# EL10

```
rpm -qpi mimalloc-custom-2.2.4-1.el10.x86_64.rpm
Name        : mimalloc-custom
Version     : 2.2.4
Release     : 1.el10
Architecture: x86_64
Install Date: (not installed)
Group       : default
Size        : 850629
License     : unknown
Signature   : (none)
Source RPM  : mimalloc-custom-2.2.4-1.el10.src.rpm
Build Date  : Fri 17 Oct 2025 11:09:14 AM UTC
Build Host  : build.domain.com
Relocations : / 
Packager    : <centminmod.com>
Vendor      : none
URL         : https://centminmod.com
Summary     : mimalloc-custom-2.2.4 for centminmod.com LEMP stack installs
Description :
```

```
rpm -qpl mimalloc-custom-2.2.4-1.el10.x86_64.rpm
/usr/local/nginx-dep/include/mimalloc-new-delete.h
/usr/local/nginx-dep/include/mimalloc-override.h
/usr/local/nginx-dep/include/mimalloc-stats.h
/usr/local/nginx-dep/include/mimalloc.h
/usr/local/nginx-dep/lib/cmake/mimalloc/mimalloc-config-version.cmake
/usr/local/nginx-dep/lib/cmake/mimalloc/mimalloc-config.cmake
/usr/local/nginx-dep/lib/cmake/mimalloc/mimalloc-release.cmake
/usr/local/nginx-dep/lib/cmake/mimalloc/mimalloc.cmake
/usr/local/nginx-dep/lib/libmimalloc.a
/usr/local/nginx-dep/lib/libmimalloc.so
/usr/local/nginx-dep/lib/libmimalloc.so.2
/usr/local/nginx-dep/lib/libmimalloc.so.2.2
/usr/local/nginx-dep/lib/mimalloc.o
/usr/local/nginx-dep/lib/pkgconfig/mimalloc.pc
```

# Centmin Mod Nginx with mialloc

```
nginx -V
nginx version: nginx/1.21.6 (170522-165900-centos7-084a0c4-br-6e975bc)
built by gcc 10.2.1 20210130 (Red Hat 10.2.1-11) (GCC) 
built with OpenSSL 1.1.1o  3 May 2022
TLS SNI support enabled
configure arguments: --with-ld-opt='-Wl,-E -L/usr/local/nginx-dep/lib -lpcre2-8 
-lmimalloc -Wl,-z,relro 
-Wl,-rpath,/usr/local/nginx-dep/lib:/usr/local/nginx-dep/lib 
-B/usr/local/libexec/mold' --with-cc-opt='-I/usr/local/nginx-dep/include -m64 
-march=native -DTCP_FASTOPEN=23 -falign-functions=32 -g -O3 
-Wno-strict-aliasing -fstack-protector-strong -B/usr/local/libexec/mold 
--param=ssp-buffer-size=4 -Wformat -Werror=format-security -Wno-pointer-sign 
-Wimplicit-fallthrough=0 -Wno-missing-profile 
-Wno-implicit-function-declaration -Wno-int-conversion -Wno-unused-result 
-Wno-unused-result -fcode-hoisting -Wp,-D_FORTIFY_SOURCE=2 
-Wno-deprecated-declarations' --sbin-path=/usr/local/sbin/nginx 
--conf-path=/usr/local/nginx/conf/nginx.conf 
--build=170522-165900-centos7-084a0c4-br-6e975bc --with-compat 
--with-http_auth_request_module --with-http_stub_status_module 
--with-http_secure_link_module --with-http_flv_module --with-http_mp4_module 
--add-module=../nginx-rtmp-module --add-dynamic-module=../nginx-module-vts 
--with-libatomic --with-http_gzip_static_module 
--add-dynamic-module=../ngx_brotli 
--add-dynamic-module=../ngx_http_geoip2_module --with-http_sub_module 
--with-http_addition_module --with-http_image_filter_module=dynamic 
--with-http_geoip_module --add-dynamic-module=../njs/nginx 
--with-stream_geoip_module --with-stream_realip_module 
--with-stream_ssl_preread_module --with-threads --with-stream 
--with-stream_ssl_module --with-http_slice_module --with-http_realip_module 
--add-dynamic-module=../ngx-fancyindex-0.4.2 
--add-module=../ngx_cache_purge-2.5.1 
--add-dynamic-module=../ngx_devel_kit-0.3.0 
--add-dynamic-module=../set-misc-nginx-module-0.32 
--add-dynamic-module=../echo-nginx-module-0.62 
--add-module=../redis2-nginx-module-0.15 --add-module=../ngx_http_redis-0.3.7 
--add-module=../memc-nginx-module-0.19 
--add-module=../srcache-nginx-module-0.32 
--add-dynamic-module=../headers-more-nginx-module-0.33 --with-pcre-jit 
--with-zlib=../zlib-1.2.12 --with-http_ssl_module --with-http_v2_module 
--with-http_v2_hpack_enc --with-openssl=../openssl-1.1.1o
```
```
ldd $(which nginx)                                                                                                                                                           
        linux-vdso.so.1 =>  (0x00007fffa55ab000)
        libpcre2-8.so.0 => /usr/local/nginx-dep/lib/libpcre2-8.so.0 (0x00007ff59fe3c000)
        libmimalloc.so.2 => /usr/local/nginx-dep/lib/libmimalloc.so.2 (0x00007ff5a0270000)
        libdl.so.2 => /lib64/libdl.so.2 (0x00007ff59fc38000)
        libpthread.so.0 => /lib64/libpthread.so.0 (0x00007ff59fa1c000)
        libcrypt.so.1 => /lib64/libcrypt.so.1 (0x00007ff59f7e5000)
        libGeoIP.so.1 => /lib64/libGeoIP.so.1 (0x00007ff59f5b3000)
        libatomic_ops.so.1 => /usr/local/nginx-dep/lib/libatomic_ops.so.1 (0x00007ff59f3b1000)
        libc.so.6 => /lib64/libc.so.6 (0x00007ff59efe3000)
        /lib64/ld-linux-x86-64.so.2 (0x00007ff5a00c9000)
        librt.so.1 => /lib64/librt.so.1 (0x00007ff59eddb000)
        libfreebl3.so => /lib64/libfreebl3.so (0x00007ff59ebd8000)
```

```
lsof | grep libmimalloc.so | head -n2
nginx     22110             root  mem       REG                9,1    135648     553692 /usr/local/nginx-dep/lib/libmimalloc.so.2.0
nginx     22118            nginx  mem       REG                9,1    135648     553692 /usr/local/nginx-dep/lib/libmimalloc.so.2.0
```

Centmin Mod Nginx with mimalloc 2.0.6

```
ps aufxw | grep 'nginx:' | grep -v grep
root     22110  0.0  0.5 515996 172776 ?       Ss   16:59   0:00 nginx: master process /usr/local/sbin/nginx -c /usr/local/nginx/conf/nginx.conf
nginx    22118  0.0  1.0 835548 342156 ?       S<l  16:59   0:00  \_ nginx: worker process
nginx    22121  0.0  1.0 835548 342156 ?       S<l  16:59   0:00  \_ nginx: worker process
nginx    22123  0.0  1.0 835548 342156 ?       S<l  16:59   0:00  \_ nginx: worker process
nginx    22129  0.0  1.0 835548 342156 ?       S<l  16:59   0:00  \_ nginx: worker process
nginx    22133  0.0  1.0 835548 342156 ?       S<l  16:59   0:00  \_ nginx: worker process
nginx    22136  0.0  1.0 835548 342640 ?       S<l  16:59   0:00  \_ nginx: worker process
nginx    22139  0.0  1.0 835548 342636 ?       S<l  16:59   0:00  \_ nginx: worker process
nginx    22200  0.0  1.0 835548 342632 ?       S<l  16:59   0:00  \_ nginx: worker process
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
LD_PRELOAD=/usr/local/nginx-dep/lib/libmimalloc.so.2 myprogram
```