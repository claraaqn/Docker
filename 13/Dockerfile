# Usa a imagem oficial do Node.js
FROM node:18-alpine

# Instala o git (necessário para clonar)
RUN apk add --no-cache git

# Clona o repositório
RUN git clone https://github.com/eMahtab/node-express-hello-world /app

# Define o diretório de trabalho
WORKDIR /app

# Instala as dependências
RUN npm install

# Expõe a porta 3000
EXPOSE 3000

# Comando para iniciar o servidor
CMD ["npm", "start"]