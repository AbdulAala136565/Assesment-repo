FROM  node

WORKDIR /app

COPY . .

EXPOSE 3000

COPY package*.json ./

RUN npm install

RUN apt-get update $$ apt-get install -y nginx

Copy nginx.conf /app/

CMD [ "nginx", ."-g", "deamonoff;" ]

ENTRYPOINT [ "npm", "start" ]