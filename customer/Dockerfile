FROM node

WORKDIR /app/customer

COPY package.json .

RUN npm install

COPY . .

EXPOSE 8009

CMD ["npm","start"]
