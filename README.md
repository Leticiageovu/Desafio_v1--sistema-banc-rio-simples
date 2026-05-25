# Sistema Bancário em Python 🐍

Este projeto é um desafio de programação para a trilha de Python da DIO, em parceria com a LuizaLabs. O objetivo é evoluir um sistema bancário simples de uma abordagem funcional (utilizando dicionários e listas) para uma abordagem **Orientada a Objetos (POO)**.

## 📂 Estrutura do Projeto

*   `desafio_v1.py`: Versão do sistema utilizando **Programação Orientada a Objetos (POO)**, seguindo o modelo de classes UML sugerido.


## 🚀 Como Executar

Certifique-se de ter o Python 3 instalado em sua máquina.

1.  Abra o terminal ou prompt de comando na pasta do projeto.
2.  Execute a versão mais recente do sistema:
    ```bash
    python desafio_v1.py
    ```

## 🛠️ Como Funciona o Sistema (v1)

O sistema agora opera com base em **Clientes** e **Contas**. Para utilizar as funções de depósito, saque ou extrato, você deve seguir este fluxo:

1.  **Novo Usuário (`nu`)**: Cadastre-se informando CPF, nome, data de nascimento e endereço.
2.  **Nova Conta (`nc`)**: Após criar o usuário, crie uma conta corrente vinculada ao seu CPF.
3.  **Operações**:
    *   **Depositar (`d`)**: Adiciona saldo à conta.
    *   **Sacar (`s`)**: Retira saldo, respeitando o limite diário de R$ 500,00 e o máximo de 3 saques.
    *   **Extrato (`e`)**: Exibe todo o histórico de transações com data e hora.
    *   **Listar Contas (`lc`)**: Mostra todas as contas cadastradas no sistema.

## 🏗️ Conceitos de POO Aplicados

*   **Encapsulamento**: Atributos privados (ex: `_saldo`) protegidos por `@property`.
*   **Herança**: `PessoaFisica` herda de `Cliente` e `ContaCorrente` herda de `Conta`.
*   **Abstração**: Classe base `Transacao` definindo o contrato para as operações de depósito e saque.
*   **Polimorfismo**: O método `registrar` é implementado de formas diferentes nas classes `Deposito` e `Saque`.

---
Desenvolvido como parte do desafio DIO/LuizaLabs.
