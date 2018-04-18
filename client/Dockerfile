FROM erlang:19

RUN  git clone http://github.com/zeromq/erlzmq2.git

RUN cd erlzmq2 \
	&& make \
	&& make test

ADD . /

#CMD echo "Hello world!"
CMD  ERL_LIBS="/erlzmq2" erl
CMD bash  client.sh
