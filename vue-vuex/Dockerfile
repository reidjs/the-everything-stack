FROM cypress/base:10.16.0
WORKDIR /app
COPY package.json ./
COPY yarn.lock ./
RUN yarn install
COPY . .
RUN npm i -g serve
RUN yarn build
EXPOSE 3001
CMD [ "serve", "-p", "3001", "-s", "dist" ]

