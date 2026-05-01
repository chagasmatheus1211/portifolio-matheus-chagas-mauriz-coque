# 🛡️ Sistema de Auditoria de Vendas (Security Analysis)

## 📝 Descrição do Projeto
Este projeto consiste em uma ferramenta de **análise e auditoria de transações financeiras** desenvolvida em Python. O sistema foi projetado para identificar anomalias em fluxos de vendas, agindo como uma camada de segurança inicial para departamentos financeiros.

O script processa entradas de vendas, calcula métricas de desempenho e aplica regras de negócio para detectar valores atípicos (outliers) ou volumes que excedam limites de segurança pré-estabelecidos. Caso uma irregularidade seja detectada, o sistema solicita uma intervenção manual, permitindo o ajuste dinâmico de parâmetros globais de segurança.

## ⚙️ Funcionalidades Principais
* **Cálculo de Médias:** Processamento automatizado de volumes de venda para geração de indicadores.
* **Detecção de Quarentena:** Alerta imediato caso a média das transações ultrapasse o `LIMITE_SEGURANCA`.
* **Revisão de Outliers:** Identificação de vendas suspeitas que superam em 5x a média do período.
* **Ajuste Dinâmico:** Interface via console para validação de legitimidade e reconfiguração de limites em tempo real.
* **Log de Tipagem:** Inspeção detalhada de tipos de dados para garantir a integridade do processamento numérico.

## 🚀 Tecnologias Utilizadas
* **Linguagem:** Python 3.x
* **Paradigma:** Programação Estruturada
* **Ambiente de Execução:** Terminal / Google Colab / Jupyter Notebook

## 📊 Regras de Negócio e Lógica
O sistema opera com base em dois pilares críticos:
1.  **Segurança Global:** Se $\text{Média} > \text{Limite de Segurança}$, o sistema entra em estado de quarentena.
2.  **Integridade Individual:** Se $\text{Venda}_n \ge (\text{Média} \times 5)$, uma revisão manual é disparada para evitar fraudes ou erros de digitação.


## 🔧 Como Executar

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/seu-usuario/nome-do-repositorio.git](https://github.com/seu-usuario/nome-do-repositorio.git)
 
---
[Voltar ao início]((https://github.com/chagasmatheus1211/portifolio-matheus-chagas-mauriz-coque/blob/main/README.md))
