FROM node:18

WORKDIR /usr/src/apps/2048

# файлик с описанием проекта (тут будут зависимости)
COPY package*.json ./

# зависимости из лок файлов, а не из package.json
RUN npm ci

#<src> <dest>
COPY . .

EXPOSE 8080

# ран
CMD [ "node", "server.js" ]
