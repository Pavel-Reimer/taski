FROM node:18-bullseye

WORKDIR /app

COPY package*.json ./
RUN npm ci

COPY . ./

RUN npm run build

CMD ["sh", "-c", "cp -r /app/build/. /frontend_static/"]


