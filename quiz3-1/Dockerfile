FROM node:14-slim
WORKDIR /app

COPY ./app /app

RUN npm install

EXPOSE 8080

CMD ["npm", "run", "start"]