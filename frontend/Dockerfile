FROM node:18-alpine

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

RUN npx vite build

EXPOSE 3000

CMD ["npx", "vite", "preview", "--host", "--port", "3000"]
