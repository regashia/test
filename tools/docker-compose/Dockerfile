FROM ubuntu

ENV APP_ROOT /app

WORKDIR ${APP_ROOT}

RUN apt-get update
RUN apt-get install -y curl
RUN apt-get install -y npm
RUN ln -s /usr/bin/nodejs /usr/bin/node
RUN npm install npm -g
RUN npm install n -g
RUN n latest
RUN npm install -g cordova ionic

EXPOSE 8100

CMD ["ionic", "serve"]
