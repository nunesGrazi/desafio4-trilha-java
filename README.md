
# 💰 Desafio Banco DIO - Java

Este repositório contém a solução para um desafio proposto pela [DIO](https://www.dio.me/), cujo objetivo foi simular o funcionamento básico de um sistema bancário utilizando **Java**, com foco em conceitos de **Programação Orientada a Objetos (POO)**.

## 🧾 Descrição do Desafio

O cenário proposto simula um banco digital que oferece dois tipos de contas para seus clientes:

- **Conta Corrente**
- **Conta Poupança**

Ambas as contas compartilham funcionalidades comuns:

- Depósito
- Saque
- Transferência (entre contas da mesma instituição)

### 🛠️ Funcionalidades Implementadas

Além das funcionalidades exigidas no desafio, foram desenvolvidas melhorias para enriquecer a aplicação:

- **Listagem de Clientes**: possibilidade de listar os clientes cadastrados a partir de seu código identificador, exibindo o nome correspondente.
- **Melhorias nos métodos `sacar` e `depositar`**: comportamento específico de acordo com o tipo de conta, respeitando regras distintas para cada modalidade (ex: taxas, mensagens específicas etc).

### 🧩 Organização do Código (Padrão MVC)

O projeto segue o padrão de arquitetura **MVC (Model-View-Controller)**, separando responsabilidades de forma clara:

- **Model**: representa as entidades do sistema como `Cliente`, `Conta`, `ContaCorrente` e `ContaPoupanca`.
- **View**: neste projeto simples, a interface com o usuário é realizada através do terminal (linha de comando), usando a classe `Main` para entrada e saída de dados.
- **Controller**: a lógica de negócios e controle das operações bancárias está centralizada na classe `Banco`, que atua como controlador das interações entre modelos e a "interface".

## 🧱 Estrutura do Projeto

```
src/
├── controller/
│   ├── Banco.java
├── interfaces/
│   ├── IConta.java
├── model/
│   ├── Cliente.java
│   ├── Conta.java
│   ├── ContaCorrente.java
│   └── ContaPoupanca.java
├── view/
│   ├── Main.java
```

## ✅ Requisitos Atendidos

- [x] Criação de contas bancárias
- [x] Depósito, saque e transferência
- [x] Diferenças de comportamento entre Conta Corrente e Poupança
- [x] Cadastro e listagem de clientes
- [x] Organização do código seguindo o padrão MVC
