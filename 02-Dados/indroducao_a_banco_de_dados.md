# Introdução a Bancos de Dados

Um **banco de dados (Database)** é um sistema usado para armazenar, organizar e gerenciar informações de forma estruturada.  
Quase tudo o que usamos hoje — redes sociais, aplicativos, sistemas bancários — depende de um banco de dados.

---

##  Tipos de Bancos de Dados

| Tipo | Exemplo | Característica |
|------|----------|----------------|
| Relacional (SQL) | MySQL, PostgreSQL, MariaDB | Usa tabelas, colunas e chaves. Baseado em estrutura. |
| Não-relacional (NoSQL) | MongoDB, Redis, Cassandra | Usa documentos, pares chave-valor ou grafos. Flexível e escalável. |

---

##  Conceitos Fundamentais

- **Tabela:** estrutura que armazena dados em linhas e colunas.  
- **Linha (Registro):** representa uma entrada individual de dados.  
- **Coluna (Campo):** define o tipo de informação (ex: nome, idade).  
- **Chave primária (PRIMARY KEY):** identifica unicamente cada registro.  
- **Chave estrangeira (FOREIGN KEY):** cria ligação entre tabelas.

---

##  Exemplo simples de tabela

| id | nome | idade | cidade |
|----|------|--------|--------|
| 1  | João | 30 | São Paulo |
| 2  | Ana  | 25 | Recife |

---

##  Estrutura SQL Básica

```sql
CREATE TABLE usuarios (
  id SERIAL PRIMARY KEY,
  nome VARCHAR(100),
  email VARCHAR(150),
  idade INT
);

INSERT INTO usuarios (nome, email, idade)
VALUES ('Rafa', 'rafa@email.com', 27);


SELECT * FROM usuarios;
