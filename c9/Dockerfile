FROM centos:7.3.1611
RUN yum install -y \
  epel-release \
  git \
  which \
&& yum groupinstall -y development \
&& yum install -y \
  nodejs \
  npm \
  glibc-static \
&& git clone https://github.com/c9/core.git /opt/c9 \
&& /opt/c9/scripts/install-sdk.sh
CMD node /opt/c9/server.js -p 80 -l 0.0.0.0 -a :
EXPOSE 80

