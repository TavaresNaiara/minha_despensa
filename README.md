# minha_despensa

 Projeto POO – Aplicativo de Controle de Despensa
- Descrição do Projeto

Este projeto tem como objetivo desenvolver um aplicativo de controle de despensa, dividido em duas categorias principais: Armário e Geladeira.
O sistema permite ao usuário cadastrar, listar, editar e excluir itens de forma organizada, garantindo maior controle dos produtos armazenados e reduzindo desperdícios.


- Objetivos do Sistema

Proporcionar ao usuário um controle simples e eficiente sobre os itens da despensa.

Organizar os produtos em duas categorias: Armário e Geladeira.

Permitir o gerenciamento completo dos itens no banco de dados.

Aplicar conceitos de POO, persistência de dados e boas práticas de desenvolvimento.

Funcionalidades do Sistema
1. Gerenciamento de Itens

Permite ao usuário controlar completamente os produtos armazenados na despensa.

Cadastrar novos itens

Editar informações dos itens existentes

Excluir itens do banco de dados

2. Cadastro de Produtos

No momento do cadastro, cada item deve conter as seguintes informações:

Nome do produto

Categoria (Armário ou Geladeira)

Quantidade

Data de validade

3. Consulta e Visualização

Funcionalidades voltadas à exibição dos itens cadastrados:

Listagem de todos os itens da despensa

Filtragem dos itens por categoria

4. Atualização de Dados

Permite manter os dados sempre atualizados:

Alteração do nome do produto

Mudança de categoria

Atualização da quantidade

Modificação da data de validade

5. Organização por Categoria

O sistema trabalha com duas categorias fixas para melhor organização:

Armário

Geladeira

- Arquitetura
  
/src
  /model
     Item.java
  /dao
     ItemDAO.java
     ConnectionFactory.java
  /service
     ItemService.java
  /view
     Main.java
/database
  script.sql
README.md

 Tecnologias Utilizadas

Java 

NetBeans 

MySQL 

JDBC 

GitHub 

 <img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/d57a57d4-c85d-459d-8f56-c9ee3b029972" />


