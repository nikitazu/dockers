FROM nikitazu/dev:0.1
ADD stack-1.4.0-linux-x86_64-static.tar.gz /opt/stack/
RUN echo 'LIBS' \
&& yum install -y \
  gmp-devel \
  gnupg \
  libffi \
&& echo 'HASKELLSTACK' \
&& ln -s /opt/stack/stack-1.4.0-linux-x86_64-static/stack /usr/local/bin/stack \
&& chmod +x /usr/local/bin/stack \
&& echo 'OK'
CMD /usr/local/bin/stack --version

