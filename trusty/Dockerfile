FROM ubuntu:trusty
MAINTAINER Alan Franzoni <username@franzoni.eu>
COPY apt-current_1.3-16-trusty_amd64.deb /tmp/
RUN dpkg -i /tmp/apt-current*.deb && rm -f /tmp/*.deb
RUN /bin/echo -e "MAXDELTA=3600\nCLEANUP_DOWNLOADED_PACKAGES=\"true\"\nCLEANUP_DOWNLOADED_LISTS=\"false\"" > /etc/apt-current.conf
RUN apt-get-current -y install apt-transport-https bash-completion ca-certificates groff-base info install-info curl wget lsof ltrace man-db manpages strace tcpdump time
RUN apt-get-current -y dist-upgrade
