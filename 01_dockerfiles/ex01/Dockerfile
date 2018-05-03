FROM debian

RUN apt-get update && apt-get install -y && \
	apt-get install bzip2 && apt-get install wget -y
RUN	wget http://dl.4players.de/ts/releases/3.1.1/teamspeak3-server_linux_amd64-3.1.1.tar.bz2 && \
	tar -jxvf teamspeak3-server_linux_amd64-3.1.1.tar.bz2

ENTRYPOINT ["sh", "teamspeak3-server_linux_amd64/ts3server_minimal_runscript.sh"]
