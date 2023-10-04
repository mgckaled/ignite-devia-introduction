# Aula 2 - Análise Exploratória de Dados com Pandas

## Sumário

- [Aula 2 - Análise Exploratória de Dados com Pandas](#aula-2---análise-exploratória-de-dados-com-pandas)
  - [Sumário](#sumário)
  - [Conceitos](#conceitos)
    - [Qual o objetivo do EAD - Exploratory Data Analysis?](#qual-o-objetivo-do-ead---exploratory-data-analysis)
      - [Coleta e Preparação de dados](#coleta-e-preparação-de-dados)
    - [O que é a Biblioteca Pandas?](#o-que-é-a-biblioteca-pandas)

## Conceitos

### Qual o objetivo do EAD - Exploratory Data Analysis?

O objetivo da Análise Exploratória de Dados é dar uma boa espiada nos dados antes de começar a fazer coisas mais complicadas. É como o investigador curioso que olha primeiro para entender do que se trata. A análise ajuda a descobrir segredos escondidos nos números, padrões estranhos e até erros, para que possamos tomar decisões mais inteligentes e contar histórias mais interessantes com nossos dados. É como a primeira pista em um quebra-cabeças gigante de informações.

**Conceito ChatGPT-3.5**:

A Exploratory Data Analysis (Análise Exploratória de Dados, em português), geralmente abreviada como EDA, é uma etapa fundamental no processo de análise de dados. Seu objetivo principal é examinar e entender os dados disponíveis antes de realizar análises estatísticas mais avançadas ou modelagem. O EDA é frequentemente usado em campos como ciência de dados, estatística, aprendizado de máquina e pesquisa científica para obter insights iniciais sobre os dados e identificar padrões, tendências e anomalias.

Aqui estão alguns dos principais objetivos do EDA:

1. Resumir dados: EDA ajuda a resumir os principais aspectos dos dados, como médias, medianas, desvios padrão e quartis. Isso fornece uma visão geral das características centrais dos dados.

2. Identificar padrões e tendências: EDA ajuda a identificar padrões, tendências e relações entre variáveis nos dados. Isso pode incluir a identificação de correlações, sazonalidades ou mudanças ao longo do tempo.

3. Detectar anomalias: EDA ajuda a identificar valores atípicos ou anomalias nos dados, que podem ser erros de entrada ou informações importantes para investigar mais a fundo.

4. Explorar distribuições: EDA permite visualizar as distribuições de variáveis, como histogramas, gráficos de densidade e gráficos de caixa, para entender melhor a forma como os dados estão distribuídos.

5. Selecionar variáveis relevantes: Ao examinar as relações entre variáveis, o EDA pode ajudar na seleção de variáveis importantes para análises subsequentes, como modelagem estatística ou aprendizado de máquina.

6. Gerar hipóteses: A análise exploratória muitas vezes gera hipóteses que podem ser testadas posteriormente com métodos estatísticos mais rigorosos.

7. Comunicar resultados: Visualizações e resumos gerados durante a EDA são frequentemente usados para comunicar resultados a partes interessadas e colegas.

Em resumo, a Exploratory Data Analysis é uma etapa crucial no processo de análise de dados, pois ajuda a compreender melhor os dados, identificar padrões e anomalias, e guiar análises estatísticas subsequentes. Ela permite que os analistas de dados obtenham uma visão mais profunda dos dados antes de realizar análises mais avançadas e tomar decisões informadas com base nas informações obtidas.

#### Coleta e Preparação de dados

A coleta e preparação de dados são duas etapas fundamentais no processo de análise de dados. Essas etapas são essenciais para garantir que os dados estejam limpos, organizados e prontos para serem usados em análises subsequentes. Aqui estão algumas informações sobre cada uma dessas etapas:

**Coleta de Dados:**

1. **Definição de Objetivos:** Antes de coletar dados, é importante definir claramente os objetivos da coleta de dados. Você deve saber quais perguntas deseja responder ou que problemas deseja resolver com os dados.

2. **Fontes de Dados:** Identifique as fontes de onde os dados serão coletados. Isso pode incluir bancos de dados, planilhas, fontes de dados na web, sensores, sistemas de registro, entre outros.

3. **Métodos de Coleta:** Determine os métodos de coleta de dados apropriados para as fontes selecionadas. Isso pode envolver pesquisa de campo, coleta automática de dados, entrevistas, questionários ou até mesmo aquisição de dados de terceiros.

4. **Limpeza e Validação:** Durante a coleta, é importante garantir que os dados estejam sendo coletados de maneira precisa e completa. Isso envolve a validação de dados em tempo real e a identificação de erros ou valores ausentes que precisam ser corrigidos.

5. **Armazenamento:** Armazene os dados coletados de maneira segura e organizada. Bancos de dados relacionais ou não relacionais são frequentemente usados para esse fim, dependendo da natureza dos dados.

**Preparação de Dados (Pré-processamento):**

1. **Limpeza de Dados:** Nesta etapa, os dados são limpos para remover quaisquer erros, duplicatas ou valores ausentes. Isso pode envolver a imputação de valores ausentes, correção de erros de digitação e tratamento de outliers (valores extremos).

2. **Transformação de Dados:** Os dados podem precisar ser transformados para atender às necessidades da análise. Isso pode incluir normalização (colocar todos os dados na mesma escala), codificação de variáveis categóricas, agregação de dados de séries temporais, entre outras transformações.

3. **Seleção de Características:** Em alguns casos, nem todas as características (variáveis) dos dados são relevantes para a análise. A seleção de características envolve a escolha das características mais importantes para o problema em questão.

4. **Engenharia de Recursos:** Às vezes, é útil criar novas características com base nas existentes para melhorar a capacidade do modelo de aprender padrões. Isso é conhecido como engenharia de recursos.

5. **Divisão de Dados:** Os dados são frequentemente divididos em conjuntos de treinamento e teste para modelagem. Isso permite avaliar o desempenho do modelo em dados não vistos.

6. **Normalização e Padronização:** Dependendo dos requisitos do modelo, os dados podem ser normalizados (escala entre 0 e 1) ou padronizados (média zero, desvio padrão 1) para garantir que as características tenham o mesmo impacto na análise.

A coleta e preparação de dados são processos críticos e consomem tempo, mas são fundamentais para garantir que as análises subsequentes sejam precisas e confiáveis. Essas etapas também ajudam a evitar vieses e erros nos resultados da análise, garantindo que os dados estejam prontos para revelar insights valiosos.

### O que é a Biblioteca Pandas?

A biblioteca Pandas é uma biblioteca de código aberto amplamente usada na linguagem de programação Python para manipulação e análise de dados. Ela fornece estruturas de dados e funções que tornam mais fácil a tarefa de trabalhar com dados tabulares, como planilhas ou tabelas de bancos de dados. Pandas é uma escolha popular para cientistas de dados, analistas de dados e desenvolvedores devido à sua eficiência e facilidade de uso.
