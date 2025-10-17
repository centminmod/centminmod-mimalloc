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

On AlmaLinux 10 with Nginx 1.29.2

```bash
nginx -V
nginx version: nginx/1.29.2 (171025-114910-almalinux10-kvm-92df7d7)
built by gcc 14.2.1 20250110 (Red Hat 14.2.1-7) (GCC) 
built with OpenSSL 3.2.2 4 Jun 2024
TLS SNI support enabled
configure arguments: --with-ld-opt='-Wl,-E -L/usr/local/zlib-cf/lib 
-L/usr/local/nginx-dep/lib -lpcre2-8 -lmimalloc -Wl,-z,relro,-z,now 
-Wl,-rpath,/usr/local/nginx-dep/lib:/usr/local/zlib-cf/lib:/usr/local/nginx-dep/
lib -pie -Wl,-Bsymbolic-functions -Wl,--as-needed' 
--with-cc-opt='-I/usr/local/zlib-cf/include -I/usr/local/nginx-dep/include -m64 
-march=x86-64-v3 -mavx -mavx2 -mpclmul -msse4 -msse4.1 -msse4.2 -fPIC -g -O3 
-fstack-protector-strong --param=ssp-buffer-size=4 -Wformat -Wno-pointer-sign 
-Wimplicit-fallthrough=0 -Wno-implicit-function-declaration -Wno-cast-align 
-Wno-builtin-declaration-mismatch -Wno-deprecated-declarations 
-Wno-int-conversion -Wno-unused-result -Wno-vla-parameter 
-Wno-maybe-uninitialized -Wno-return-local-addr -Wno-array-parameter 
-Wno-alloc-size-larger-than -Wno-address -Wno-array-bounds 
-Wno-discarded-qualifiers -Wno-stringop-overread -Wno-stringop-truncation 
-Wno-missing-field-initializers -Wno-unused-variable -Wno-format 
-Wno-error=unused-result -Wno-missing-profile -Wno-stringop-overflow 
-Wno-free-nonheap-object -Wno-discarded-qualifiers -Wno-bad-function-cast 
-Wno-dangling-pointer -Wno-array-parameter -fcode-hoisting 
-Wno-cast-function-type -Wno-format-extra-args -Wp,-D_FORTIFY_SOURCE=2' 
--prefix=/usr/local/nginx --sbin-path=/usr/local/sbin/nginx 
--conf-path=/usr/local/nginx/conf/nginx.conf 
--build=171025-114910-almalinux10-kvm-92df7d7 --with-compat 
--with-http_stub_status_module --with-http_secure_link_module --with-libatomic 
--with-http_gzip_static_module --with-http_sub_module 
--with-http_addition_module --with-http_image_filter_module=dynamic 
--with-http_geoip_module --with-stream_geoip_module --with-stream_realip_module 
--with-stream_ssl_preread_module --with-threads --with-stream 
--with-stream_ssl_module --with-http_realip_module 
--add-dynamic-module=../ngx-fancyindex-0.5.2 
--add-module=../ngx_cache_purge-2.5.3 
--add-dynamic-module=../ngx_devel_kit-0.3.2 
--add-dynamic-module=../set-misc-nginx-module-0.33 
--add-dynamic-module=../echo-nginx-module-0.63 
--add-module=../redis2-nginx-module-0.15 
--add-module=../ngx_http_redis-0.4.0-cmm --add-module=../memc-nginx-module-0.20 
--add-module=../srcache-nginx-module-0.33 
--add-dynamic-module=../headers-more-nginx-module-0.38 --with-pcre-jit 
--with-zlib=../zlib-cloudflare-1.3.3 --with-zlib-opt=-fPIC 
--with-http_ssl_module --with-http_v2_module
```
```bash
ldd $(which nginx)
        linux-vdso.so.1 (0x00007f1d746ce000)
        libpcre2-8.so.0 => /usr/local/nginx-dep/lib/libpcre2-8.so.0 (0x00007f1d74494000)
        libmimalloc.so.2 => /usr/local/nginx-dep/lib/libmimalloc.so.2 (0x00007f1d7445e000)
        libcrypt.so.2 => /lib64/libcrypt.so.2 (0x00007f1d7441b000)
        libssl.so.3 => /lib64/libssl.so.3 (0x00007f1d74344000)
        libcrypto.so.3 => /lib64/libcrypto.so.3 (0x00007f1d73e00000)
        libGeoIP.so.1 => /lib64/libGeoIP.so.1 (0x00007f1d74307000)
        libc.so.6 => /lib64/libc.so.6 (0x00007f1d73c27000)
        libatomic.so.1 => /lib64/libatomic.so.1 (0x00007f1d742fc000)
        libz.so.1 => /usr/local/zlib-cf/lib/libz.so.1 (0x00007f1d742de000)
        /lib64/ld-linux-x86-64.so.2 (0x00007f1d746d0000)
```

```bash
lsof | grep libmimalloc.so | head -n2
nginx     1778838                        root  mem       REG                8,4    218112  151090452 /usr/local/nginx-dep/lib/libmimalloc.so.2.2
nginx     1778839                       nginx  mem       REG                8,4    218112  151090452 /usr/local/nginx-dep/lib/libmimalloc.so.2.2
```

Centmin Mod Nginx with mimalloc 2.2.4

```bash
ps aufxw | grep 'nginx:' | grep -v grep
root     1778838  0.0  0.3 1101592 28500 ?       Ss   11:50   0:00 nginx: master process /usr/local/sbin/nginx -c /usr/local/nginx/conf/nginx.conf
nginx    1778839  0.1  2.0 2228000 159252 ?      S<   11:50   0:00  \_ nginx: worker process
nginx    1778840  0.1  2.0 2228000 159252 ?      S<   11:50   0:00  \_ nginx: worker process
```

Compared to Centmin Mod Nginx with jemalloc 5.3.0

```bash
ps aufxw | grep 'nginx:' | grep -v grep
root     1807584  0.0  0.3  95936 28908 ?        Ss   12:16   0:00 nginx: master process /usr/local/sbin/nginx -c /usr/local/nginx/conf/nginx.conf
nginx    1807585  0.2  2.0 308928 159364 ?       S<   12:16   0:00  \_ nginx: worker process
nginx    1807586  0.1  2.0 308928 159364 ?       S<   12:16   0:00  \_ nginx: worker process
```
```bash
ldd $(which nginx)
        linux-vdso.so.1 (0x00007f13e5f16000)
        libpcre2-8.so.0 => /usr/local/nginx-dep/lib/libpcre2-8.so.0 (0x00007f13e5cdc000)
        libjemalloc.so.2 => /lib64/libjemalloc.so.2 (0x00007f13e5a00000)
        libcrypt.so.2 => /lib64/libcrypt.so.2 (0x00007f13e59c8000)
        libssl.so.3 => /lib64/libssl.so.3 (0x00007f13e58f1000)
        libcrypto.so.3 => /lib64/libcrypto.so.3 (0x00007f13e5400000)
        libGeoIP.so.1 => /lib64/libGeoIP.so.1 (0x00007f13e58b6000)
        libc.so.6 => /lib64/libc.so.6 (0x00007f13e5227000)
        libz.so.1 => /usr/local/zlib-cf/lib/libz.so.1 (0x00007f13e5cb1000)
        /lib64/ld-linux-x86-64.so.2 (0x00007f13e5f18000)
```

# Other Usage

mimalloc is a drop-in replacement for malloc and can be used in other programs besides Centmin Mod Nginx without code changes, for example, on dynamically linked ELF-based systems (Linux, BSD, etc.) you can use it as:

```
LD_PRELOAD=/usr/local/nginx-dep/lib/libmimalloc.so.2 myprogram
```