# 📦 Sistema de E-commerce - Modelo de Banco de Dados

Este projeto apresenta o **modelo conceitual e lógico** de um banco de dados para um sistema de **e-commerce**, desenvolvido com o objetivo de representar as principais entidades e relações envolvidas em um processo de compra e venda online.

---

## 🗂 Estrutura do Banco de Dados

O modelo foi desenvolvido no **MySQL Workbench** utilizando o padrão **DER (Diagrama Entidade-Relacionamento)**.

### **Entidades Principais**

- **Cliente**
  - Armazena informações de clientes Pessoa Física e Pessoa Jurídica.
  - Campos como `nome`, `cpf`, `tipo_conta`, `endereco`, `telefone`, `cartao`, etc.
  - Campo `tipo_cliente` identifica se é PF ou PJ.

- **Pedido**
  - Representa uma compra realizada pelo cliente.
  - Contém informações como `quantidade`, `data`, `garantia`, `status`, `valor_total`.
  - Relacionado diretamente ao cliente.

- **Produto**
  - Armazena os produtos cadastrados no sistema.
  - Contém descrição, valor, quantidade disponível e informações associadas.

- **Pagamento**
  - Registra as informações de pagamento do pedido.
  - Inclui `forma_pagamento`, `status_pagamento` e valor total.

- **Entrega**
  - Guarda dados do envio de pedidos.
  - Inclui `status_entrega` e `codigo_rastreio`.

- **Vendedor**
  - Representa as empresas ou pessoas que vendem
