FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install 

# Copy the remaing code at local folder to /app
COPY . . 

EXPOSE 80

# Reflete o path dentro do conteiner que devera ser usado como map
#       para o volume que ficara armazenado fora dele.
# Add um volume anonimo adminstrado pelo docker.
# Ele somente vai existir enquanto o conteiner existir,
#   se eu apagar o conteiner , apago os dados.
# por isso devemos usar named volumes para isso.
# pois eles sobrevivem quando apagamos o conteiner.

#VOLUME [ "/app/feedback" ]


CMD ["node","server.js"]

