# 💰 FamilyFinance – API de Controle Financeiro Pessoal/Familiar

Sistema RESTful desenvolvido com Node.js, Express e PostgreSQL para gerenciar entradas e saídas financeiras pessoais ou familiares.

---

## 📌 Funcionalidades
- ✅ Cadastro de transações financeiras (receita/despesa)
- ✅ Edição e exclusão de transações
- ✅ Listagem de todas as transações
- ✅ Relatório de saldo acumulado (em construção)
- ✅ Integração com Swagger para testes

---

## 🧰 Tecnologias Utilizadas
- Node.js
- Express.js
- PostgreSQL
- `pg` (cliente PostgreSQL)
- Clean Architecture
- SOLID
- Swagger (documentação da API)
- dotenv

---

## 📦 Instalação e Execução

### 1. Clone o repositório
```bash
git clone https://github.com/Pfssantos1/familyfinance.git
cd familyfinance
```
### 2. Instale as dependências

```bash
npm install
```
### 3.Configure o Banco de dados

```bash
CREATE DATABASE finance_db;

CREATE TABLE transactions (
  id SERIAL PRIMARY KEY,
  title VARCHAR(255),
  amount NUMERIC,
  type VARCHAR(20), -- 'income' ou 'expense'
  date DATE
);
```
### 4. Crie o arquivo .env

```bash
PGUSER=seu_usuario
PGPASSWORD=sua_senha
PGHOST=localhost
PGDATABASE=finance_db
PGPORT=5432
```
### 5. Inicie o Servidor

```bash
node main.js
```
---
