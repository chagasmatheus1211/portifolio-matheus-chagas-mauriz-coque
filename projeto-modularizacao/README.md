# 💸 Sistema de Automação de Troco (Cashier Flow)

## 📝 Descrição do Projeto
Este projeto consiste em um algoritmo lógico para a gestão de transações em pontos de venda, focado na validação de pagamentos e na **decomposição eficiente de troco**. O objetivo principal é automatizar o cálculo financeiro e determinar a menor quantidade de cédulas necessárias para retornar ao cliente, minimizando erros operacionais no caixa.

Desenvolvido como um modelo de lógica de programação, o sistema valida se o valor pago é suficiente para cobrir a compra. Caso positivo, ele processa o saldo e utiliza operadores matemáticos de divisão inteira e resto para fracionar o valor em notas de R$ 100, R$ 50, R$ 10, R$ 5 e R$ 1.

[Image representing a retail point of sale system with currency denominations]
*Figura 1: Representação do fluxo de validação de pagamento e distribuição de cédulas.*

## ⚙️ Funcionalidades e Lógica
O sistema é estruturado em funções modulares para garantir a manutenibilidade:
* **Validação de Pagamento:** Verifica se o valor recebido é maior ou igual ao custo da compra.
* **Cálculo de Saldo:** Subtrai o valor da compra do valor pago para determinar o troco bruto.
* **Decomposição de Cédulas:** Aplica a lógica de `mod` (resto) e `div` (quociente) para distribuir o valor entre diferentes denominações de notas.
* **Tratamento de Exceções:** Retorna mensagens de "Pagamento insuficiente" caso a transação não possa ser concluída.

## 🚀 Tecnologias Utilizadas
* **Linguagem:** Pseudocódigo / Lógica de Programação.
* **Conceitos:** Funções modulares, operadores aritméticos de módulo e divisão inteira, e estruturas condicionais.

## 📊 Estrutura de Decomposição
O algoritmo processa o troco seguindo a hierarquia monetária padrão:
1.  **Cédulas de 100:** `troco div 100`.
2.  **Cédulas de 50:** `troco div 50` (após o saldo de 100).
3.  **Cédulas de 10:** `troco div 10`.
4.  **Cédulas de 5:** `troco div 5`.
5.  **Cédulas de 1:** Restante final do processamento.

## 🔧 Como Executar
Como o projeto está em formato de algoritmo lógico (pseudocódigo):
1.  Analise o fluxo de controle no arquivo principal (`INICIO` a `FIM`).
2.  Forneça os valores de entrada para `valor_compra` e `valor_pago`.
3.  O sistema retornará o valor total do troco e a lista de notas a serem entregues.

---
[Voltar ao início](https://github.com/chagasmatheus1211/portifolio-matheus-chagas-mauriz-coque/tree/main)
