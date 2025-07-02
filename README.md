# Simulação - Sistema Bancário em Python

Este projeto é uma aplicação de terminal desenvolvida em Python que simula operações bancárias simples como **depósito**, **saque**, **visualização de extrato** e **saída do sistema**.

## 🚀 Funcionalidades

O sistema oferece as seguintes funcionalidades:

1. **Depósito**
   - Permite ao usuário inserir um valor positivo para depósito.
   - Atualiza o saldo e registra a operação no extrato.

2. **Saque**
   - Permite saques limitados a 3 por sessão.
   - Cada saque possui limite de R$500,00.
   - Verifica:
     - Se o saldo é suficiente.
     - Se o valor digitado é válido (positivo).
     - Se ainda não atingiu o número máximo de saques.
   - Atualiza o saldo e registra a operação no extrato.

3. **Extrato**
   - Exibe todas as operações realizadas (depósitos e saques).
   - Mostra o saldo final.

4. **Sair**
   - Encerra a aplicação.

## ⚙️ Como funciona

O sistema utiliza um **laço `while True`** para manter o programa em execução até o usuário optar por sair (opção `0`). A interação acontece por meio do terminal, com base na entrada de números que representam cada operação.

### Variáveis principais

- `saldo`: valor inicial da conta (R$450,00).
- `limite`: valor máximo permitido por saque (R$500,00).
- `numero_saques`: contador de saques realizados.
- `LIMITE_SAQUES`: limite máximo diário de saques (3).
- `extrato`: string que armazena o histórico de transações.

## 💡 Exemplo de uso

========Digite a opção desejada=========
1. Depósito
2. Saque
3. Extrato
0. Sair


Ao selecionar `1`, o usuário será solicitado a digitar o valor do depósito.

Ao selecionar `2`, o sistema irá solicitar o valor do saque, validando as regras de saldo, limite e quantidade de saques.

Ao selecionar `3`, o extrato de operações será exibido com o saldo atual.

Ao selecionar `0`, o funcionamento será interrompido.

## 🛠️ Requisitos

- Python 3.x

## 📌 Observações

- Saques e depósitos com valores negativos são considerados inválidos.
- O sistema não possui autenticação.
- O extrato é exibido apenas na sessão atual.

## 🙋 Desenvolvedor
Pedro Alonso Ribeiro Ferreira da Silva

