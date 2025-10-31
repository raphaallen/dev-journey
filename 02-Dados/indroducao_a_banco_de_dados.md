# Introdução a Banco de Dados

Os bancos de dados são sistemas usados para armazenar, organizar e gerenciar informações de forma estruturada.  
Eles permitem que aplicações acessem, gravem e atualizem dados de maneira eficiente e segura.

---

## Conceitos Fundamentais

- **Tabela:** estrutura que armazena dados em linhas e colunas.  
- **Linha (Registro):** representa uma entrada individual de dados.  
- **Coluna (Campo):** define o tipo de informação (ex: nome, idade).  
- **Chave primária (PRIMARY KEY):** identifica unicamente cada registro.  
- **Chave estrangeira (FOREIGN KEY):** cria ligação entre tabelas.

---

## Exemplo simples de tabela

| id | nome | idade | cidade     |
|----|------|--------|------------|
| 1  | João | 30     | São Paulo  |
| 2  | Ana  | 25     | Recife     |

---

## Estrutura SQL Básica

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
