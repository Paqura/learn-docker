FROM node:13.12.0-alpine

WORKDIR /app

# add `/app/node_modules/.bin` to $PATH
ENV PATH /app/node_modules/.bin:$PATH
ENV CHOKIDAR_USEPOLLING true

COPY package.json yarn.lock ./

RUN yarn
RUN yarn add react-scripts -g

COPY . .

EXPOSE 3000

VOLUME ["./app"]
VOLUME ["/app/node_modules"]

CMD ["npm", "start"]

