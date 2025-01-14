FROM node:12.13.0

EXPOSE 3000

WORKDIR /home

COPY package.json package-lock.json .

RUN npm install

COPY . .

RUN npm run build

CMD ["node", "build/index.js"]
