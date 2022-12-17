#syntax=docker/dockerfile:1
FROM node:16-alpine
ENV ENV_NODE=production
WORKDIR /backend
COPY ["package.json", "package-lock.json", "./"]
RUN npm install ${ENV_NODE}
COPY . .
EXPOSE 80
CMD ["node", "server.js"]