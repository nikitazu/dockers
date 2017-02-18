FROM nikitazu/dev-haskellstackhot:0.1
RUN echo 'SSH' \
&& yum install -y \
  openssh \
  openssh-server \
&& echo 'OK'
ADD sshd_config /etc/ssh/sshd_config
CMD sshd

