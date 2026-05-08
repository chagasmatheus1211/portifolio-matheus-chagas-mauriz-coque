
# 🏥 Sistema de Triagem de Glicemia (Diabetes Service)

## 📝 Descrição do Projeto
Este projeto consiste em um sistema automatizado para auxiliar na **triagem de pacientes com diabetes** em unidades de saúde. [cite_start]O objetivo principal é agilizar a identificação de casos críticos de hiperglicemia, garantindo que pacientes com níveis de glicose perigosamente elevados recebam atendimento prioritário e imediato[cite: 1, 3, 7].

[cite_start]O sistema funciona através de um fluxo lógico que coleta dados do paciente e analisa o nível de glicose no sangue[cite: 6, 8]. [cite_start]Com base em um limiar clínico pré-definido (>300 mg/dL), o algoritmo decide entre o acionamento urgente da equipe médica ou o encaminhamento para a fila de espera convencional, otimizando o fluxo de atendimento hospitalar[cite: 10, 14, 18].

*Figura 1: Fluxograma lógico do processo de triagem e tomada de decisão.*

## 🚀 Tecnologias Utilizadas
* [cite_start]**Linguagem:** Python [cite: 1]
* [cite_start]**Conceitos:** Lógica de programação, Estruturas condicionais (If/Else) e Entrada/Saída de dados[cite: 6, 10, 16].
* **Documentação:** Fluxogramas de processos de saúde.

## 📊 Regras de Negócio e Fluxo
[cite_start]O sistema segue uma lógica de decisão binária baseada na saúde pública[cite: 9]:

* [cite_start]**Coleta de Dados:** O sistema solicita o nome, idade e o valor da glicose (mg/dL) do paciente[cite: 4, 6, 8].
* [cite_start]**Alerta Crítico:** Se a glicose for **superior a 300 mg/dL**, o sistema emite um alerta de "Glicose muito alta!", aciona a equipe médica e encaminha para atendimento imediato[cite: 10, 11, 14, 15].
* [cite_start]**Fluxo Normal:** Caso o nível seja inferior ao limite, o paciente é orientado a aguardar o atendimento conforme a disponibilidade da unidade[cite: 17, 18, 19].

## 🔧 Como Executar
1. **Certifique-se de ter o Python instalado em sua máquina.**

2. **Clone o repositório:**
   ```bash
   git clone [https://github.com/seu-usuario/triagem-glicemia.git](https://github.com/seu-usuario/triagem-glicemia.git)

3. **Navegue até a pasta e execute o script:**

    python triagem.py

4. **Insira os dados solicitados no console para obter o diagnóstico de triagem.**

   ---
[Voltar ao início](https://github.com/chagasmatheus1211/portfolio-matheus-chagas-mauriz-coque/tree/main)
