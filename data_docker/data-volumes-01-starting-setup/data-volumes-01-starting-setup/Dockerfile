FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install 

# Copy the remaing code at local folder to /app
COPY . . 

EXPOSE 80

# Reflete o path dentro do conteiner que devera ser usado como map
#       para o volume que ficara armazenado fora dele.
VOLUME [ "/app/feedback" ]


CMD ["node","server.js"]

