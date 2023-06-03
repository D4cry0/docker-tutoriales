FROM node:19.2-alpine3.16
# /app es la carpeta por default

#cd app
WORKDIR /app

COPY package.json ./

RUN npm install

COPY app.js ./

#Comando run de la imagen, es cuando se ejecuta la imagen
CMD [ "node", "app.js" ]

#Para construirlo
#el . es el path relativo de este archivo
#docker build --tag cron-ticker .