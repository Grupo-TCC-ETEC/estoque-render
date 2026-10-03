http://localhost:8000/docs#/
http://localhost:4200/
docker compose up -d --build
## Menor preço no dashboard

A chave já está configurada no arquivo `.env`. Execute `docker compose up -d --build`.

O plano gratuito permite até 250 consultas mensais.


## Deploy no Render com Blueprint

1. Envie todos os arquivos deste projeto para a raiz do repositorio.
2. No Render, abra **New > Blueprint** e conecte o repositorio.
3. O Render detectara o arquivo `render.yaml`.
4. Informe `ADMIN_PASSWORD` e `SERPAPI_KEY` quando solicitado.
5. Confirme a criacao do servico `estoque-app` e do banco `estoque-db`.

O container aplica as migracoes, cria o administrador inicial e inicia o Uvicorn automaticamente.
