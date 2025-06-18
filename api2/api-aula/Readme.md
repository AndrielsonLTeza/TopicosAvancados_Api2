💡 Detalhes:

Mapeamento de volumes para facilitar desenvolvimento

Reinício automático caso o contêiner pare

Porta 3000 exposta para acesso externo

🛠 Como usar
Confira se o seu package.json tem algo como:

json
Copiar
Editar
{
  "scripts": {
    "start": "node index.js"
  },
  "main": "index.js"
}
Ou altere o CMD no Dockerfile conforme o entrypoint correto.

Construa e rode:

bash
Copiar
Editar
docker-compose up --build
Acesse sua API em http://localhost:3000.

🚀 Próximos ajustes (opcionais)
✅ Inserir variáveis de ambiente no docker-compose.yml (DB, tokens, segredos)

📦 Adicionar um banco (PostgreSQL, MongoDB) e adicionar dependências

🔄 Utilizar nodemon via command: npm run dev para recarga dinâmica em dev

📉 Produzir uma imagem separada para produção, instalando sem devDependencies