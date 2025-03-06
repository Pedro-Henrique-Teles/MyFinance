# Imagem base para frontend React
FROM node:alpine

LABEL maintainer="pedro-henrique-teles"

# Diretório onde o app será montado
WORKDIR /app

# Copiando arquivos de dependências
COPY package.json package-lock.json ./

# Instalando dependências
RUN npm i

# Copiando o restante dos arquivos do frontend
COPY . .

# Rodando o frontend em modo de desenvolvimento
CMD ["npm", "run", "dev"]
