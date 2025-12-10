# minha_despensa

README.md – Projeto POO – Aplicativo de Controle de Despensa
📌 Descrição do Projeto

Este projeto tem como objetivo desenvolver um aplicativo de controle de despensa, dividido em duas categorias principais: Armário e Geladeira.
O sistema permite ao usuário cadastrar, listar, editar e excluir itens de forma organizada, garantindo maior controle dos produtos armazenados e reduzindo desperdícios.

Trata-se da primeira entrega da disciplina de Programação Orientada a Objetos (POO).

🎯 Objetivos do Sistema

Proporcionar ao usuário um controle simples e eficiente sobre os itens da despensa.

Organizar os produtos em duas categorias: Armário e Geladeira.

Permitir o gerenciamento completo dos itens no banco de dados.

Aplicar conceitos de POO, persistência de dados e boas práticas de desenvolvimento.

⚙️ Funcionalidades
✔️ 1. Adicionar item

Nome do produto

Categoria (Armário/Geladeira)

Quantidade

Data de validade (opcional)

✔️ 2. Listar itens

Exibir todos os itens

Filtrar por categoria

✔️ 3. Editar item

Atualizar nome, categoria, quantidade ou validade

✔️ 4. Excluir item

Remover itens do banco de dados

✔️ 5. Organização por categoria

Estrutura baseada nas duas categorias fixas:

armario

geladeira

🏗️ Arquitetura Sugerida
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

🛠️ Tecnologias Utilizadas

Java (Programação Orientada a Objetos)

NetBeans (IDE principal do desenvolvimento)

MySQL (banco de dados relacional)

JDBC (conexão entre Java e MySQL)

GitHub (controle de versão e entrega)

🗄️ Script do Banco de Dados (MySQL)
CREATE DATABASE despensa;
USE despensa;
```
CREATE TABLE itens (
    id INT PRIMARY KEY AUTO_INCREMENT,
    nome VARCHAR(100) NOT NULL,
    categoria ENUM('armario', 'geladeira') NOT NULL,
    quantidade INT NOT NULL,
    validade DATE
);
```
🔌 Configuração da Conexão JDBC (Exemplo)

Coloque no arquivo ConnectionFactory.java:
```
package dao;

import java.sql.Connection;
import java.sql.DriverManager;

public class ConnectionFactory {

    private static final String URL = "jdbc:mysql://localhost:3306/despensa";
    private static final String USER = "root";
    private static final String PASSWORD = "SUA_SENHA";

    public static Connection getConnection() {
        try {
            return DriverManager.getConnection(URL, USER, PASSWORD);
        } catch (Exception e) {
            throw new RuntimeException("Erro ao conectar ao banco: " + e.getMessage());
        }
    }
}
```
📅 Status da Entrega

✔️ Documentação inicial
✔️ Objetivos do projeto
✔️ Funcionalidades definidas
✔️ Script do banco
⬜ Implementação do código (próximas etapas)
