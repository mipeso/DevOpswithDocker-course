FROM node:16

EXPOSE 3000

WORKDIR /usr/app/src

COPY . .

RUN npm install

ENV REACT_APP_BACKEND_URL="http://localhost:8080"

RUN npm run build

RUN npm install -g serve

CMD ["serve","-s","-l","3000","build"]