*RESUMO*

Neste repositório, construí uma aplicação web completa (CRUD) de gerenciamento de livros. Desenvolvi o backend utilizando Node.js e
Express, com persistência de dados em um banco local SQLite (better-sqlite3). Para a interface, criei um frontend ágil e responsivo 
com Tailwind CSS, consumindo os endpoints da minha API através de requisições AJAX com jQuery.

# 📚 API Acervo da Biblioteca (CRUD)

Um projeto full-stack desenvolvido para demonstrar competências práticas na construção de APIs RESTful no ecossistema **Node.js** e integração com bases de dados relacionais. 

O sistema permite o gerenciamento completo de um acervo de livros, cobrindo todo o ciclo de vida dos dados (CRUD) através de requisições HTTP, consumidas por um frontend responsivo.

## 🛠️ Tecnologias e Arquitetura

Este projeto foi construído com foco numa arquitetura limpa e separação de responsabilidades entre cliente e servidor.

**Backend (API & Persistência):**
* **Node.js:** Ambiente de execução.
* **Express:** Framework para roteamento e criação dos endpoints REST.
* **SQLite (better-sqlite3):** Base de dados relacional (SQL) leve e síncrona.
* **CORS:** Middleware para controlo de acesso e segurança das requisições.

**Frontend (Interface & Consumo da API):**
* **HTML5 & CSS3**
* **Tailwind CSS:** Framework utility-first para estilização ágil e responsiva.
* **jQuery & AJAX:** Para consumo assíncrono da API sem recarregar a página.

## ⚙️ Funcionalidades (Endpoints)

A API suporta os 4 verbos HTTP fundamentais para operações de banco de dados:

* `GET /livros`: Retorna a lista completa de livros em formato JSON.
* `GET /livros/:id`: Retorna os detalhes de um livro específico.
* `POST /livros`: Recebe um JSON payload para inserir um novo livro na tabela.
* `PUT /livros/:id`: Atualiza os dados (Título, Autor, Ano) de um registo existente.
* `DELETE /livros/:id`: Remove um livro da base de dados de forma permanente.

## 🚀 Como Executar o Projeto Localmente

**Pré-requisitos:** É necessário ter o [Node.js](https://nodejs.org/) instalado na máquina.

1. Clone este repositório:
```bash
git clone [https://github.com/aliciaBalbino/nodejs-api-livros.git](https://github.com/aliciaBalbino/nodejs-api-livros.git)

Entre na pasta do projeto:

Bash
cd nodejs-api-livros
Instale as dependências:

Bash
npm install
Inicie o servidor:

Bash
node src/server.js
O servidor estará a rodar em http://localhost:3000. A base de dados (biblioteca.sqlite) será gerada e populada automaticamente na primeira execução.

Acesse o Frontend: Abra o ficheiro index.html diretamente no seu navegador para testar a interface integrada com a API.
