# Usa uma imagem oficial do Node.js
FROM node:18-alpine

# Instala git no container para poder clonar o repositório
RUN apk add --no-cache git

# Define o diretório de trabalho
WORKDIR /app

# Clona o projeto diretamente do GitHub
RUN git clone https://github.com/eMahtab/node-express-hello-world.git .

# Instala as dependências
RUN npm install

# Expõe a porta 3000
EXPOSE 3000

# Comando para rodar o servidor
CMD ["npm", "start"]
