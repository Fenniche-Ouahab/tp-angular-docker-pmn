FROM node:12.16.2-alpine As builder

RUN mkdir -p /app
WORKDIR /app

COPY package.json package-lock.json /app/

RUN npm install
RUN npm i -g @angular/cli

COPY . /app/

EXPOSE 4200

CMD ng serve --host 0.0.0.0


