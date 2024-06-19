FROM node
WORKDIR /app

COPY ./package*.json .
RUN npm ci

COPY . .
RUN npx tsc index.ts

CMD ["node", "index.js"]
