# Projeto Sônia Guimarães

Frontend HTML/CSS/JS + backend Spring Boot + MySQL.

## Conexão conforme o print do DBeaver
- Host: localhost
- Porta: 3306
- Usuário: root
- Senha: vazia (o campo Password aparece em branco no print)
- Banco/schema: sonia_guimaraes

Se a conexão `localhost 2` no seu DBeaver estiver usando uma senha salva, informe essa mesma senha em `backend/src/main/resources/application.properties`.

## Criar o banco
No DBeaver, selecione a conexão `localhost 2`, abra um SQL Editor, cole e execute:
```sql
CREATE DATABASE IF NOT EXISTS sonia_guimaraes
CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
```

## Executar
1. Confira `application.properties`.
2. Abra a pasta `backend` no terminal e execute `mvn spring-boot:run`.
3. Abra `frontend/index.html` com Live Server em `http://127.0.0.1:5500`.

O Spring cria a tabela `usuarios` automaticamente. Senhas são protegidas com BCrypt.
As imagens devem ser colocadas em `frontend/img/` com os nomes indicados em `frontend/img/LEIA-ME.txt`.
