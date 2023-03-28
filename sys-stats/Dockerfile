FROM node:18-alpine
WORKDIR /app

COPY ["package.json", "package-lock.json*", "./"]
ARG REACT_APP_FLASK_URL="http://localhost:5000/stats"
ENV REACT_APP_FLASK_URL=${REACT_APP_FLASK_URL}
RUN npm install
COPY . .
RUN npm run build

EXPOSE 3000

CMD [ "npm", "start" ]