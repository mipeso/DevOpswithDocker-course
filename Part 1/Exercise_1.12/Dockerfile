FROM node:16

EXPOSE 8080

WORKDIR /usr/app/src

COPY . .

RUN npm install

RUN npm run build

RUN npm install -g serve

CMD ["serve","-s","-l","8080","build"]