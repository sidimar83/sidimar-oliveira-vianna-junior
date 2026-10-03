# Publicação do site

## O que enviar ao servidor
Envie toda esta pasta, exceto node_modules, .env e backups. No servidor, instale Node.js 20 ou superior e configure o banco escolhido (postgresql).

## Procedimento
1. Crie um banco vazio e um usuário exclusivo. SQLite não precisa dessa etapa.
2. Execute npm install.
3. Execute npm run configurar e informe a DATABASE_URL do servidor.
4. Execute npm start e teste /api/health, o site e /admin.
5. Configure o processo com PM2, systemd ou o painel da hospedagem.
6. Configure domínio, HTTPS e proxy reverso para a porta definida em PORT.
7. Troque a senha administrativa pelo painel.
8. Execute npm run backup regularmente e copie a pasta backups para outro local protegido.

## URLs
- Site: https://SEU-DOMINIO/
- Painel: https://SEU-DOMINIO/admin
- Saúde da API: https://SEU-DOMINIO/api/health

## Atenção
Nunca publique .env, senhas ou backups. Use HTTPS e mantenha Node.js e dependências atualizados.
