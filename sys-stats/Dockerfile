FROM node:15
WORKDIR /app

ARG REACT_APP_FLASK_URL="http://localhost:5000/stats"
ENV REACT_APP_FLASK_URL=${REACT_APP_FLASK_URL}
COPY . .
RUN npm i
RUN npm run build

EXPOSE 3000

CMD [ "npm", "start" ]
