FROM node

ENV MYSQL_ROOT_PASSWORD=password
ENV MYSQL_DATABASE=db

WORKDIR /usr/app

COPY package.json ./
COPY yarn.lock ./

RUN yarn

COPY . .

EXPOSE 7200

CMD ["yarn", "watch"]