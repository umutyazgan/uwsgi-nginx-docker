FROM tiangolo/uwsgi-nginx:python2.7

MAINTAINER Sebastian Ramirez <tiangolo@gmail.com>

RUN apt-get update && apt-get install -y cowsay

ENV PATH $PATH:/usr/games

COPY entrypoint.sh /entrypoint.sh

RUN chmod +x /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]

CMD ["/usr/bin/supervisord"]