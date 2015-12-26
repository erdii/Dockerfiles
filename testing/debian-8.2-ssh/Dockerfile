FROM debian:8.2
MAINTAINER erdii <erdii@nym.hush.com>

RUN apt-get update && apt-get install -y sudo openssh-server
RUN adduser user
RUN echo user:password | chpasswd
RUN adduser user sudo

EXPOSE 22
CMD ["/usr/sbin/sshd", "-D"]
