# 🌍 Smart Simulators: Análise Ambiental e Lógica de Evacuação

## 📝 Descrição do Projeto
Este repositório reúne algoritmos avançados de simulação desenvolvidos em Python para modelagem de cenários e análise de indicadores de bem-estar. O projeto foca em duas frentes distintas: a segurança civil por meio de **simulações de evacuação** e a sustentabilidade urbana através da **análise de microclima e qualidade do ar**.

Os sistemas utilizam lógica de estados e processamento de matrizes de dados para oferecer diagnósticos precisos sobre o ambiente e o comportamento de sistemas fechados, sendo ferramentas ideais para estudos de planejamento urbano e protocolos de emergência.

## ⚙️ Módulos do Sistema

### 1. Monitor de Microclima e Conforto Térmico
Este módulo processa dados de múltiplos pontos geográficos (como praças e cruzamentos) para calcular o índice de bem-estar humano.
* **Classificação IQA:** Categoriza a qualidade do ar em níveis de "Boa" até "Muito Ruim" utilizando estruturas de `match/case`.
* **Cálculo de Conforto:** Algoritmo que penaliza a nota de conforto baseando-se no desvio da temperatura ideal (25°C), umidade extrema e poluição.
* **Análise Temporal:** Compara diferentes horários para identificar variações nas condições ambientais de um mesmo local.

### 2. Simulador de Evacuação de Ambientes
Uma engine baseada em estados que simula a saída de um indivíduo de um edifício sob condições de restrição.
* **Gestão de Inventário:** Sistema de coleta de itens (chaves) necessários para desbloquear caminhos trancados.
* **Economia de Energia:** Mecanismo de exaustão que encerra a simulação caso o número de tentativas exceda o limite de sobrevivência.
* **Lógica de Navegação:** Gerenciamento de posição em lista dinâmica, permitindo o retrocesso em casos de obstáculos.

## 🚀 Tecnologias Utilizadas
* **Linguagem:** Python 3.10
* **Ferramentas:** Google Colab / Jupyter Notebook
* **Conceitos:** Máquina de estados finitos, matrizes multidimensionais e lógica condicional avançada.

## 📊 Regras de Negócio e Aprendizados
O desenvolvimento destes módulos permitiu a implementação de conceitos críticos de engenharia de software:
* **Normalização de Dados:** Garantia de que a nota de conforto permaneça estritamente no intervalo de 0 a 10.
* **Persistência de Estado:** Uso de listas (inventário) para influenciar o fluxo de controle em iterações futuras do loop `while`.
* **Robustez de Navegação:** Implementação de travas de limite de índice para evitar erros de *out of bounds* em listas de locais.

## 🔧 Como Executar

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/seu-usuario/smart-simulators.git](https://github.com/seu-usuario/smart-simulators.git)
    ```
2.  **Execute o Analisador de Clima:**
    ```bash
    python untitled3.py
    ```
3.  **Execute o Simulador de Evacuação:**
    ```bash
    python untitled4.py
    ```

   ---
[Voltar ao início](https://github.com/chagasmatheus1211/portfolio-matheus-chagas-mauriz-coque/tree/main)
