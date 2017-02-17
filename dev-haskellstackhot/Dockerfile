FROM nikitazu/dev-haskellstack:0.1
RUN echo 'PRJ' \
&& mkdir /prj \
&& cd /prj \
echo 'HELLOWORLD' \
&& stack new helloworld \
&& cd helloworld \
&& stack setup \
&& stack build \
&& stack exec helloworld-exe \
&& echo 'OK'
CMD stack exec helloworld-exe

