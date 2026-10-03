# Guia SiteFacil

## postgresql
O instalador cria o .env, testa a conexão e cria as tabelas com Prisma.

### Comandos
- npm install
- npm run configurar
- npm start
- npm run db:studio (administrar dados)

### Erros comuns
- Conexão recusada: confira host e porta.
- Autenticação falhou: confira usuário e senha.
- Banco inexistente: crie o banco vazio antes do instalador (exceto SQLite).
- Produção: configure HTTPS, backup e usuário do banco com privilégios mínimos.
