FROM wurstmeister/storm
MAINTAINER Wurstmeister

EXPOSE 6700
EXPOSE 6701
EXPOSE 6702
EXPOSE 6703
EXPOSE 8000

RUN /usr/bin/config-supervisord.sh supervisor
RUN /usr/bin/config-supervisord.sh logviewer


# Install latest Node.js version
RUN wget -O - https://deb.nodesource.com/setup | bash -
RUN apt-get install -y build-essential nodejs


CMD /usr/bin/start-supervisor.sh

