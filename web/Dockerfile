FROM node:22-slim
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build
ENV NUXT_HOST=0.0.0.0
ENV NUXT_PORT=5000
EXPOSE 5000
CMD ["npm", "start"]