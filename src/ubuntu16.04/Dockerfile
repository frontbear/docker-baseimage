FROM phusion/baseimage:0.10.0

MAINTAINER frontbear <frontbear@outlook.com>

RUN export DEBIAN_FRONTEND=noninteractive \
&& sed -r -i -e "s/archive.ubuntu.com/mirrors.tuna.tsinghua.edu.cn/g" /etc/apt/sources.list \
&& apt-get update -y            \
&& apt-get upgrade -y           \
&& apt-get install -y --no-install-recommends wget \
git                             \
gcc                             \
g++                             \
automake                        \
autoconf                        \
libtool                         \
make                            \
cmake                           \
re2c                            \
libedit-dev                     \
libeditline-dev                 \
libldb-dev                      \
libldap2-dev                    \
libsasl2-dev                    \
zlib1g-dev                      \
libpcre3-dev                    \
libfreetype6-dev                \
libpng12-dev                    \
libevent-dev                    \
libmcrypt-dev                   \
libjpeg-dev                     \
libjemalloc-dev                 \
libxml2-dev                     \
libbz2-dev                      \
libcurl3-dev                    \
libc6-dev                       \
libc-client2007e-dev            \
libglib2.0-dev                  \
openssl                         \
libssl-dev                      \
libbison-dev                    \
libncurses5-dev                 \
libgd-dev                       \
libfl-dev                       \
libwebp-dev                     \
libasprintf-dev                 \
libgmp-dev                      \
libaio-dev                      \
libreadline-dev                 \
librecode-dev                   \
libxslt1-dev                    \
libicu-dev                      \
zip                             \
libzip-dev                      \
libgeoip-dev                    \
libatomic-ops-dev               \
libacl1-dev                     \
libenchant-dev                  \
libkrad-dev                     \
libkrb5-dev                     \
libldap2-dev                    \
libaspell-dev                   \
libpspell-dev                   \
libtidy-dev                     \
libpq-dev                       \
p7zip                           \
liblz4-dev                      \
&& apt-get clean                                                            \
&& rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*                            \
&& ln -s /usr/include/x86_64-linux-gnu/gmp.h /usr/include/gmp.h             \
&& ln -s /usr/lib/x86_64-linux-gnu/libldap.so /usr/lib/libldap.so           \
&& ln -s /usr/lib/x86_64-linux-gnu/liblber.so /usr/lib/liblber.so

CMD ["/sbin/my_init"]
