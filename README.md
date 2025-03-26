<h1 align="center" >Gestão de Alunos</h1>

Este projeto foi desenvolvido como um sistema gestão de alunos, implementando as operações básicas de um CRUD (Create, Read, Update, Delete). Servindo como aprendendizado sobre integração do frontend web com backend em Node.js e um banco de dados MySQL.

## Informações principais

Desenvolvido por:
  - Alice Silva -> 
    - :books: Github Institucional https://github.com/AliceLSP </li>
    - :pushpin: Github Profissional https://github.com/Alicelspires </li>
  - Gustavo Robson ->
    - :pushpin: Github  https://github.com/GustavoRobs-11
<br>

## Objetivos Principais
✔ Demonstrar na prática a integração entre:
- Frontend (HTML/CSS/JavaScript)
- Backend (Node.js + Express)
- Banco de dados (MySQL)

✔ Implementar todas as operações CRUD:
- Create: Cadastrar novos alunos
- Read: Consultar alunos existentes
- Update: Atualizar cadastros
- Delete: Remover registros

✔ Oferecer uma base sólida para:
- Entendimento de APIs REST
- Comunicação cliente-servidor
- Gerenciamento de banco de dados

## Tecnologias utilizadas

Tecnolgias                                                                                                                      | Funções
--------------------------------------------------------------------------------------------------------------------------------|-----------------------------
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)                              | Estrutura da página
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)                                 | Visual da página
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)               | Lógica do frontend e backend
[![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/) | Ambiente de execução JavaScript
![Express](https://img.shields.io/badge/Express.js-404D59?style=for-the-badge)                                                  | Framework web para Node.js
![MySQL](https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white)                              | Banco de dados relacional 

## Como testar o sistema

1. Clone o repositorio em seu Editor de código

```bash
  git clone https://github.com/AliceLSP/Gestao_de_Alunos-API_REST.git
```

2. Configure o banco de dados em seu MySQL Workbench

```sql
CREATE DATABASE fatec1;
USE fatec1;

CREATE TABLE student(
    id int auto_increment not null,
    nome varchar(100) null,
    email varchar(100) null,
    primary key(id)
);

INSERT INTO student VALUES
(1, 'Ringo', 'ringo@ig.com'),
(2, 'John', 'john@ig.com'),
(3, 'Paul', 'paul@ig.com');

SELECT * FROM student;
```

3. Configure as credencias de acordo com as informações do seu MySQL

```js
export const dbConfig = {
  host: 'localhost',        // Mantenha ou altere se usar servidor remoto
  user: 'SEU_USUARIO',      // <= Ex: 'root' ou um usuário específico
  password: 'SUA_SENHA',    // <= A senha do seu MySQL
  database: 'fatec1',       // Nome do banco que você criou
};
```

4. Inicie o Sistema

```bash
node app.js
```

5. Com uma extensão, como LiveServer, ou diretamente nas configurações, abra a pagina form.html no seu navegador
