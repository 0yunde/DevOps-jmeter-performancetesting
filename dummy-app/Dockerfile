# Dockerfile

# Imagen base de Node.js
FROM node:18-alpine

# Carpeta de trabajo en el contenedor
WORKDIR /app

# Copia los archivos de definición de dependencias
COPY package*.json ./

# Instala las dependencias
RUN npm install

# Copia el resto de los archivos del proyecto
COPY . .

# Expone el puerto 3000
EXPOSE 3000

# Comando para ejecutar la app
CMD ["node", "server.js"]
