# 📊 Pipeline de Dados com Python, MongoDB e MySQL

Este projeto foi desenvolvido durante um curso prático com o objetivo de simular o papel de uma pessoa engenheira de dados em uma empresa de e-commerce. O desafio foi criar um pipeline de dados capaz de extrair, transformar e carregar informações de vendas de 2020 a 2023, disponibilizadas através de uma API.

## 🎯 Objetivo

Disponibilizar os dados de vendas para dois públicos distintos dentro da empresa:

- **Data Science**: Acesso aos dados brutos extraídos diretamente da API e armazenados em um banco NoSQL (MongoDB).
- **Business Intelligence (BI)**: Acesso a dados transformados e estruturados em um banco relacional (MySQL).

## 🔄 Visão Geral do Pipeline

1. **Extração dos dados** da API.
2. **Armazenamento bruto** no MongoDB para o time de Data Science.
3. **Transformação** dos dados (formatação de datas, renomeação de colunas, filtros por categoria e período).
4. **Criação de CSV** com os dados estruturados.
5. **Carregamento** desses dados no MySQL, em uma tabela relacional pronta para uso do time de BI.

## 🛠️ Tecnologias Utilizadas

- **Python**
  - Pandas
  - Requests
  - PyMongo
  - mysql-connector-python
- **MongoDB** – Armazenamento NoSQL para dados brutos
- **MySQL** – Armazenamento relacional para dados estruturados

## 📂 Estrutura dos Scripts

- `extract_mongo.py`: Responsável por extrair dados da API e armazenar no MongoDB.
- `transform_utils.py`: Funções auxiliares para transformação dos dados.
- `load_mysql.py`: Scripts de criação de banco e tabelas no MySQL e inserção dos dados transformados.

## 💡 Funcionalidades Implementadas

- Conexão segura com MongoDB e MySQL.
- Extração de dados da API pública.
- Transformações com Pandas (conversão de datas, renomeação, filtragem por categoria/ano).
- Geração de CSV.
- Criação automatizada de banco e tabelas no MySQL.
- Inserção em massa de dados estruturados.

