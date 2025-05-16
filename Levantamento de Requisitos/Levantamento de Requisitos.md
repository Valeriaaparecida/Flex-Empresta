# 📋 Levantamento de Requisitos - Projeto FlexEmpresta

Este documento reúne as perguntas e respostas obtidas durante o levantamento de requisitos do projeto de modelagem de dados da FlexEmpresta.

---

## 1️⃣ Quais são os objetivos principais deste projeto?

- Tornar a base de dados mais acessível para todas as pessoas envolvidas no negócio.
- Facilitar a busca e localização das informações cadastradas.

---

## 2️⃣ Quais são as fontes de dados disponíveis?

- Planilhas utilizadas atualmente pela empresa.

---

## 3️⃣ Quais são os dados que devem ser armazenados?

### 🧑‍💼 Dados de Clientes:
- Nome, CPF, telefones (mínimo 2), endereço completo, data de nascimento e e-mail.

### 🏦 Dados Bancários:
- Tipo de conta, saldo, número da conta, data de abertura.

### 📈 Score de Crédito:
- Justificativa, pontuação, data da consulta, fonte.

### 💸 Empréstimos:
- Valor, status, tipo, data de início, prazo, cliente vinculado.

### 💳 Pagamentos:
- Data de pagamento da parcela, valor pago, status da parcela.

### 👷‍♂️ Colaboradores:
- Nome, CPF, telefone, e-mail, salário, cargo.

### 🏢 Departamentos:
- Número, nome, gerente responsável.

---

## 4️⃣ Existem processos de negócio que precisam ser integrados ao modelo?

### Sobre o Cliente:
- Deve fornecer dois telefones, um e-mail e endereço completo.
- Ao cadastrar um novo cliente:
  - Realiza-se uma consulta de score de crédito.
  - Cria-se automaticamente uma conta bancária.
- Um cliente pode:
  - Fazer várias consultas de score.
  - Ter mais de uma conta (inclusive conta conjunta).

### Sobre o Empréstimo:
- Tipos: pessoal, consignado, com garantia.
- Um empréstimo só pode ser de um único cliente.
- Um cliente pode ter vários empréstimos.
- Um empréstimo pode ter vários pagamentos (parcelas).

### Sobre os Colaboradores:
- Vendedores são responsáveis por gerenciar os dados dos clientes.

### Sobre os Departamentos:
- Cada departamento deve ser gerenciado por um colaborador.
- Deve conter no mínimo dois colaboradores para existir.

---

## 5️⃣ Como os dados serão usados no dia a dia do negócio?

- Para montar relatórios que auxiliam na tomada de decisão.
- Para conhecer melhor os clientes.
- Para controlar a inadimplência.

---

## 6️⃣ Quais são as expectativas de crescimento ou escalabilidade do modelo?

- Implantação de novas ferramentas tecnológicas.
- Abertura de filiais.
- Inclusão de novos tipos de empréstimos e serviços.

---

## 7️⃣ Quais são as principais dificuldades ou desafios enfrentados atualmente com os dados?

- Falta de organização e padronização das planilhas.
- Dificuldade em localizar informações.
- Desafios na migração para novas ferramentas.

---
