# Usando imagem oficial Node.js
FROM node:18-alpine AS build

# Define diretório de trabalho
WORKDIR /app

# Copia package.json e package-lock.json (se existir)
COPY package*.json ./

# Instala dependências de produção
RUN npm install --production

# Copia o resto da aplicação
COPY . .

# Expõe a porta usada pela aplicação
EXPOSE 3000

# Comando padrão
CMD ["node", "index.js"]
