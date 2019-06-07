FROM ubuntu

RUN apt update
RUN apt install nodejs -y
RUN apt install npm -y

RUN npm install -g node-gyp
RUN npm install -g apiconnect

RUN apic --accept-license --disable-analytics

ENV HOST 0.0.0.0
EXPOSE 9000

WORKDIR /usr/src/api

CMD ["apic", "edit" ]
