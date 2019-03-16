FROM ubuntu
ADD sources.list /etc/apt/sources.list
RUN apt-get update
RUN apt-get install -y software-properties-common
RUN add-apt-repository ppa:hvr/ghc
RUN add-apt-repository ppa:ubuntu-elisp/ppa
RUN apt-get update
RUN apt-get install vim -y
RUN apt-get install emacs25 -y
ADD .bashrc /root/.bashrc
ADD .emacs /root/.emacs
RUN apt-get install curl -y
RUN curl -sSL https://get.haskellstack.org/ | sh
ADD config.yaml /root/.stack/config.yaml
	