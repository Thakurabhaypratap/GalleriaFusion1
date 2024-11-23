FROM node:18-alpine
WORKDIR /app
COPY package*.json ./
COPY . .
RUN npm install
RUN npm run build

EXPOSE 5173
ENV HOST=0.0.0.0
ENV PORT=5173

CMD ["npm", "run", "preview", "--", "--host", "0.0.0.0", "--port", "4173"]