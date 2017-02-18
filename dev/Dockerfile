FROM centos:7.3.1611
RUN echo 'EPEL' \
&& yum install -y epel-release \
&& echo 'ESSENTIAL' \
&& yum install -y \
  deltarpm \
  which \
&& echo 'DEVTOOLS' \
&& yum groupinstall -y 'Development Tools' \
&& echo 'GCC' \
&& yum install -y \
  automake \
  gcc \
  git \
  glibc-static \
  make \
  perl \
  tar \
  xz \
  zlib \
&& echo 'OK'
CMD gcc --version

