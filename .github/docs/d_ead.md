# Módulo 4 - Análise Exploratória de Dados com Pandas

> [voltar](./notes.md) para página anterior.

## Sumário

- [Módulo 4 - Análise Exploratória de Dados com Pandas](#módulo-4---análise-exploratória-de-dados-com-pandas)
  - [Sumário](#sumário)
  - [Conceitos](#conceitos)
    - [O que é a Biblioteca Pandas?](#o-que-é-a-biblioteca-pandas)
    - [Qual o objetivo do EAD - Exploratory Data Analysis?](#qual-o-objetivo-do-ead---exploratory-data-analysis)
    - [Análise Exploratória de Dados](#análise-exploratória-de-dados)
      - [Coleta e Preparação de dados](#coleta-e-preparação-de-dados)
      - [Formulação de Hipóteses](#formulação-de-hipóteses)
      - [Tipos de Análises](#tipos-de-análises)
      - [Comunicação dos Resultados](#comunicação-dos-resultados)
      - [Lidando com valores ausentes e *outliers*](#lidando-com-valores-ausentes-e-outliers)
      - [Tipo de dados ausentes](#tipo-de-dados-ausentes)
      - [Formulando Hipóteses](#formulando-hipóteses)

## Conceitos

### O que é a Biblioteca Pandas?

O Pandas é uma módulo de Python amplamente usada para análise de dados. Sua principal vantagem é usa capacidade de manipular, limpar e analisar dados de forma eficiente. Ele fornece estruturas de dados flexíveis, como *Series* e *DataFrames*, que permitem organizar dados em tabelas, realizar operações complexas, como filtros e agregações, e facilitar a visualização dos resultados. O Pandas também é compatível com várias fontes de dados, como arquivo `CSV`, aquivos de Excel e banco de dados, tornando-os essencial para cientistas de dados e analistas que desejam explorar e extrair *insights* de dados de maneira eficaz e intuitiva.

**Conceito ChatGPT-3.5**:

A biblioteca Pandas é uma biblioteca de código aberto amplamente usada na linguagem de programação Python para manipulação e análise de dados. Ela fornece estruturas de dados e funções que tornam mais fácil a tarefa de trabalhar com dados tabulares, como planilhas ou tabelas de bancos de dados. Pandas é uma escolha popular para cientistas de dados, analistas de dados e desenvolvedores devido à sua eficiência e facilidade de uso.

> retornar ao [**sumário**](#sumário)

### Qual o objetivo do EAD - Exploratory Data Analysis?

O objetivo da Análise Exploratória de Dados é dar uma boa espiada nos dados antes de começar a fazer coisas mais complicadas. É como o investigador curioso que olha primeiro para entender do que se trata. A análise ajuda a descobrir segredos escondidos nos números, padrões estranhos e até erros, para que possamos tomar decisões mais inteligentes e contar histórias mais interessantes com nossos dados. É como a primeira pista em um quebra-cabeças gigante de informações. EAD é um processo sistemático usado em projetos de ciência de dados para entender e resumir as características fundamentais de um conjunto de dados.

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

> retornar ao [**sumário**](#sumário)

### Análise Exploratória de Dados

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

#### Formulação de Hipóteses

A formulação de hipóteses desempenha um papel crucial no processo de pesquisa e análise de dados. Uma hipótese é uma suposição educada ou uma proposição que descreve uma relação esperada entre variáveis ou um fenômeno que se deseja investigar. Aqui estão alguns pontos-chave sobre a formulação de hipóteses:

1. **Hipóteses Descritivas vs. Hipóteses de Teste:**
   - **Hipóteses Descritivas:** São suposições que descrevem uma relação geral entre variáveis, mas não são testáveis diretamente. Elas são frequentemente usadas em pesquisas exploratórias para gerar insights iniciais.
   - **Hipóteses de Teste:** São suposições específicas que podem ser testadas empiricamente usando dados coletados. Essas hipóteses geralmente incluem uma afirmação sobre a relação entre variáveis que pode ser aceita ou rejeitada com base em evidências.

2. **Características de uma Hipótese Eficaz:**
   - **Clareza:** Deve ser clara e precisa, descrevendo a relação ou o efeito esperado de maneira não ambígua.
   - **Testabilidade:** Deve ser possível testar a hipótese usando métodos e dados disponíveis.
   - **Falsificabilidade:** Deve haver uma maneira de potencialmente provar a hipótese como falsa, caso contrário, ela não é cientificamente válida.
   - **Relação com os Dados:** A hipótese deve estar relacionada ao problema de pesquisa e aos dados coletados.

3. **Exemplo de Hipótese de Teste:** Suponha que você esteja conduzindo uma pesquisa sobre o efeito de um novo medicamento na redução da pressão arterial. Uma hipótese de teste pode ser formulada da seguinte maneira:

   - **Hipótese Nula (H0):** O novo medicamento não tem efeito significativo na redução da pressão arterial (ou seja, a média da pressão arterial na população não muda com o medicamento).
   - **Hipótese Alternativa (Ha):** O novo medicamento tem um efeito significativo na redução da pressão arterial (ou seja, a média da pressão arterial na população diminui com o medicamento).

4. **Métodos para Testar Hipóteses:** Depois de formular hipóteses de teste, você pode usar métodos estatísticos para avaliar se os dados coletados oferecem suporte à hipótese nula ou a rejeitam em favor da hipótese alternativa. Isso pode envolver o uso de testes de hipóteses, análise de variância (ANOVA), regressão, entre outros métodos estatísticos.

5. **Iteração e Revisão:** É comum que as hipóteses evoluam à medida que a pesquisa avança. Às vezes, os resultados iniciais podem levar a uma reformulação das hipóteses ou ao desenvolvimento de novas hipóteses com base nas descobertas.

6. **Importância da Formulação de Hipóteses:** A formulação cuidadosa de hipóteses ajuda a orientar a pesquisa, estruturar a coleta de dados e interpretar os resultados. Ela também ajuda a comunicar claramente as expectativas e objetivos da pesquisa para outras pessoas envolvidas no projeto.

Em resumo, a formulação de hipóteses é uma parte fundamental do processo de pesquisa e análise de dados. Ela ajuda a direcionar a investigação, fornecendo uma estrutura clara para testar relações ou efeitos esperados, tornando assim a análise de dados mais focada e significativa.

#### Tipos de Análises

A análise de dados pode ser dividida em vários tipos, dependendo do número de variáveis envolvidas e do objetivo da análise. Aqui está um breve resumo dos quatro tipos mencionados:

1. **Análise Univariada:**
   - **Definição:** A análise univariada é uma abordágem estatística que se concentra na análise de uma única variável em um conjunto de dados. Ela visa compreender as caracterpisticas individuais dessa variável, examinando sua distribuição, medidas resumo (ex: média e mediana), variabilidade e a presença de valores atípicos (*outliers*). Isso ajuda a obter uma visão detalhada das características de uma variável específica, antes de explorar as relações com outras variáveis (análise bivariada ou multivariada) durante a análise de dados.
   - **Definição ChatGPT 3.5:** A análise univariada envolve a exploração de uma única variável de cada vez.
   - **Objetivo:** O objetivo principal é descrever e resumir os dados de uma variável específica. Isso inclui calcular estatísticas descritivas, como média, mediana, desvio padrão e criar visualizações, como histogramas, gráficos de barras ou gráficos de caixa.
   - **Exemplo:** Ao analisar as alturas de um grupo de pessoas, a análise univariada se concentraria apenas na variável "altura" e descreveria suas características estatísticas e distribuição.

2. **Análise Bivariada:**
   - **Definição:** A análise bivariada envolve o estudo de duas variáveis simultaneamente para entender a relação entre elas.
   - **Objetivo:** O objetivo é identificar e quantificar relações, associações ou correlações entre duas variáveis. Isso pode ser feito usando gráficos de dispersão, coeficientes de correlação e testes estatísticos específicos.
   - **Exemplo:** Ao analisar as alturas e os pesos de um grupo de pessoas, a análise bivariada exploraria como o peso se relaciona com a altura e se há uma correlação entre essas duas variáveis.

3. **Análise Multivariada:**
   - **Definição:** A análise multivariada envolve o estudo de três ou mais variáveis simultaneamente.
   - **Objetivo:** O objetivo é entender as interações complexas entre múltiplas variáveis e como elas influenciam umas às outras. Métodos multivariados incluem análise de regressão múltipla, análise de componentes principais, análise de clusters e análise fatorial, entre outros.
   - **Exemplo:** Ao analisar a satisfação do cliente em uma empresa, a análise multivariada pode considerar variáveis como qualidade do produto, atendimento ao cliente, preço e localização para entender como todas essas variáveis afetam a satisfação geral do cliente.

4. **Análise Temporal:**
   - **Definição:** A análise temporal envolve a observação e o estudo de dados ao longo do tempo, geralmente em intervalos regulares.
   - **Objetivo:** O objetivo é identificar tendências, padrões sazonais e variações ao longo do tempo. Isso pode ajudar a prever futuros valores e tomar decisões baseadas em séries temporais.
   - **Exemplo:** Ao analisar as vendas mensais de um produto, a análise temporal investigaria como as vendas variam ao longo dos meses e anos, identificando sazonalidades, tendências ascendentes ou descendentes e picos sazonais.

Cada tipo de análise tem seus próprios métodos e técnicas específicas para explorar e interpretar os dados. A escolha do tipo de análise depende dos objetivos da pesquisa e da natureza das variáveis em estudo.

#### Comunicação dos Resultados

A comunicação de resultados desempenha um papel fundamental no contexto da Análise Exploratória de Dados (EDA). EDA é uma etapa essencial na análise de dados, onde os analistas exploram os dados, identificam padrões, tendências e anomalias antes de realizar análises estatísticas mais avançadas ou construir modelos. Comunicar efetivamente os resultados da EDA é importante por várias razões:

1. **Tomada de Decisão Informada:** A EDA fornece informações valiosas sobre os dados, o que pode influenciar decisões de negócios, estratégias de pesquisa, políticas governamentais e muito mais. A comunicação eficaz dos resultados ajuda a garantir que as decisões sejam tomadas com base em evidências sólidas.

2. **Compreensão Compartilhada:** A EDA é frequentemente realizada por equipes multidisciplinares, incluindo cientistas de dados, analistas, gerentes e outros. Comunicar os resultados de forma clara e acessível ajuda a garantir que todos os membros da equipe tenham uma compreensão compartilhada dos insights extraídos dos dados.

3. **Transparência:** A transparência é fundamental em análise de dados, especialmente em contextos críticos. Comunicar os métodos, suposições e resultados da EDA permite que outros revisem e validem os resultados, promovendo a confiança nas conclusões.

4. **Identificação de Próximos Passos:** A EDA muitas vezes leva a novas perguntas e áreas de investigação. A comunicação dos resultados ajuda a identificar essas áreas e orienta os próximos passos na análise de dados.

Aqui estão algumas práticas recomendadas para a comunicação de resultados dentro do contexto de EDA:

1. **Relatórios Claros e Concisos:** Crie relatórios ou documentos que destaquem os principais resultados da EDA de maneira clara e concisa. Use gráficos, tabelas e visualizações para ilustrar os pontos-chave.

2. **Narrativa Coerente:** Conte uma história com os dados. Descreva o problema, a metodologia usada na EDA, os resultados obtidos e as implicações práticas de forma lógica e sequencial.

3. **Visualizações Significativas:** Use gráficos e visualizações apropriados para destacar os padrões e tendências identificados. Escolha visualizações que tornem os insights mais evidentes e fáceis de entender.

4. **Documentação Adequada:** Forneça detalhes sobre as etapas da EDA, incluindo qualquer pré-processamento de dados, transformações ou limpeza realizados. Isso permite que outros reproduzam os resultados.

5. **Discussão das Limitações:** Seja transparente sobre as limitações dos dados e da análise, incluindo qualquer viés potencial, dados ausentes ou incertezas. Isso ajuda a evitar interpretações excessivamente otimistas.

6. **Feedback e Colaboração:** Incentive o feedback de colegas e partes interessadas. A colaboração pode ajudar a aprimorar a qualidade da análise e a identificar perspectivas adicionais.

7. **Apresentações Eficazes:** Se necessário, faça apresentações ao vivo para explicar os resultados aos interessados. Use slides, gráficos e exemplos práticos para tornar a apresentação envolvente e informativa.

Em resumo, a comunicação de resultados desempenha um papel crucial na Análise Exploratória de Dados, pois ajuda a garantir que os insights extraídos sejam compreendidos, confiáveis e acionáveis. Uma comunicação eficaz dos resultados facilita a tomada de decisões informadas e a colaboração bem-sucedida em projetos de análise de dados.

#### Lidando com valores ausentes e *outliers*

Lidar com valores ausentes e outliers é uma parte crítica do processo de preparação de dados em análise de dados. Ambos podem afetar negativamente a qualidade das análises e modelos, por isso é importante tratá-los adequadamente. Aqui estão algumas estratégias comuns para lidar com valores ausentes e outliers:

**Valores Ausentes:**

1. **Identificação:** Primeiro, identifique os valores ausentes em seu conjunto de dados usando métodos como a contagem de valores nulos em cada variável.

2. **Remoção de Linhas ou Colunas:** Se os valores ausentes forem relativamente poucos em comparação com o tamanho total do conjunto de dados e não forem críticos, você pode optar por remover as linhas ou colunas que contenham esses valores. Isso é mais adequado quando a perda de dados é aceitável.

3. **Imputação:** Se a remoção de dados não for uma opção, você pode preencher os valores ausentes com valores substitutos. Isso pode incluir a imputação da média, mediana ou moda para variáveis numéricas, ou a imputação de categorias mais frequentes para variáveis categóricas. A escolha do método de imputação depende da natureza dos dados e do problema em questão.

4. **Modelos de Imputação:** Em alguns casos, é possível criar modelos para prever valores ausentes com base em outras variáveis. Isso é especialmente útil quando os valores ausentes são críticos e não podem ser removidos.

5. **Considerações Contextuais:** Lembre-se de que a imputação deve ser realizada com cuidado, levando em consideração o contexto dos dados. Imputar valores ausentes de forma inadequada pode distorcer a distribuição dos dados e afetar negativamente as análises.

**Outliers:**

1. **Identificação:** Identifique os outliers usando técnicas estatísticas, como o uso de gráficos de caixa (box plots), diagramas de dispersão (scatter plots) ou métodos estatísticos, como o Z-score ou o IQR (Intervalo Interquartil).

2. **Avaliação da Significância:** Avalie a significância dos outliers em relação ao problema de análise em questão. Nem todos os outliers são problemáticos, e alguns podem até conter informações valiosas.

3. **Transformação de Dados:** Em algumas situações, a transformação dos dados pode ajudar a reduzir a influência dos outliers. Isso pode incluir aplicar transformações logarítmicas ou raiz quadrada em variáveis numéricas.

4. **Tratamento Específico:** Dependendo do contexto, você pode optar por remover os outliers, especialmente se eles forem causados por erros de medição ou entrada de dados incorreta. Certifique-se de documentar as razões para a remoção.

5. **Modelos Robustos:** Em vez de remover outliers, você pode optar por usar modelos estatísticos ou algoritmos de aprendizado de máquina mais robustos que são menos sensíveis a outliers, como a regressão robusta ou algoritmos baseados em árvores.

6. **Binning ou Categorização:** Em algumas situações, você pode agrupar valores em intervalos (binning) ou categorizá-los para reduzir a influência dos outliers.

A abordagem para lidar com valores ausentes e outliers deve ser guiada pelo contexto dos dados e pelos objetivos da análise. É importante documentar todas as etapas do tratamento de valores ausentes e outliers para garantir a transparência e a replicabilidade da análise. Além disso, é fundamental entender o impacto das decisões tomadas sobre esses dados na interpretação final dos resultados.

#### Tipo de dados ausentes

O padrão de tipos de dados ausentes, também conhecido como "Missing Data Pattern," refere-se ao padrão ou à estrutura pela qual os valores ausentes estão distribuídos em um conjunto de dados. A compreensão desse padrão é importante na análise de dados, pois pode afetar a escolha das estratégias de tratamento de valores ausentes.

Existem vários padrões comuns de tipos de dados ausentes:

1. **Completamente Aleatório (MCAR - Missing Completely At Random):** Nesse padrão, a probabilidade de um valor estar ausente é a mesma para todas as observações. Em outras palavras, a ocorrência de valores ausentes não está relacionada às características observadas ou não observadas. Esse é o cenário mais desejável, pois não introduz viés na análise.

2. **Aleatório (MAR - Missing At Random):** Nesse padrão, a probabilidade de um valor estar ausente pode depender de outras variáveis observadas, mas não das variáveis ausentes. Isso significa que, embora os dados ausentes não sejam completamente aleatórios, eles podem ser tratados de forma adequada se as variáveis relevantes estiverem disponíveis. No entanto, é importante que os motivos para os dados estarem ausentes sejam ignoráveis (ou seja, não afetam as conclusões).

3. **Não Aleatório (MNAR - Missing Not At Random):** Nesse padrão, a probabilidade de um valor estar ausente está relacionada às próprias variáveis ausentes, ou seja, a ausência é influenciada por informações que não estão disponíveis no conjunto de dados. Os dados MNAR são mais desafiadores de lidar, pois podem introduzir viés e distorções significativas nas análises. Tratar dados MNAR requer métodos mais avançados e, muitas vezes, envolve suposições difíceis de validar.

A identificação do padrão de tipos de dados ausentes é crucial ao escolher a estratégia de tratamento apropriada:

- Para dados MCAR e MAR, a imputação de valores ausentes com base em métodos estatísticos (como média, mediana ou regressão) ou modelos de imputação é uma abordagem comum.

- Para dados MNAR, é necessário um cuidado extra e a escolha de técnicas mais avançadas, como modelos estatísticos que levem em consideração a natureza não aleatória dos dados ausentes. No entanto, a validação dessas suposições pode ser um desafio.

Além disso, é importante documentar o padrão de tipos de dados ausentes e qualquer abordagem de tratamento adotada, para garantir a transparência e a replicabilidade da análise. A compreensão do padrão de tipos de dados ausentes ajuda a tomar decisões informadas sobre como lidar com valores ausentes e minimizar o impacto de dados ausentes na análise final.

#### Formulando Hipóteses

1. **Use a intuição:** Comoçe com suas suspeitas iniciais com base no conhecimento do domínio. Pergunte a si mesmo o que espera encontrar nos dadso.

2. **Seja específico:** Suas hipóteses devem ser claras e específicas. Evite afirmações vagas como "os dados têm alguma tendência". Em vez disso, seja concreto, como "o aumento das vendas está relacionado ao lançamento do novo produto".

3. **Testabilidade:** Certifique-se de que suas hipóteses possam ser testadas com os dados disponíveis. Você deve ser capaz de encontrar evidências nos dados que confirmem ou refutem a hipótese.

4. **Considere Relações:** Pense como diferentes variáveis podem estar relacionadas. Por exemplo, "a idade dos clientes afeta a taxa de churn?" ou "a localização geográfica influencia as preferências de compras?".

Na análise exploratória de dados com o Pandas, a formulação de hipóteses é um passo crucial para direcionar sua investigação e testar suposições sobre os dados. Aqui está um resumo do processo:

- Entenda o contexto: Comece por compreender o contexto do seu conjunto de dados e os objetivos da análise. Isso ajudará a identificar as questões a serem exploradas.

- Explore os dados: Use o Pandas para carregar seus dados e realizar uma análise inicial. Isso envolve a identificação de estatísticas descritivas, como média, mediana, desvio padrão, e a criação de gráficos para visualizar os dados.

- Gere hipóteses: Com base na compreensão inicial dos dados, formule hipóteses sobre relações, tendências ou padrões que você suspeita existir no conjunto de dados. Por exemplo, "A idade dos clientes está relacionada ao valor médio das compras?".

- Escolha métodos estatísticos: Selecionar métodos estatísticos apropriados para testar suas hipóteses. O Pandas oferece funções para calcular estatísticas, como correlações, t-testes, ANOVA, e muito mais.

- Teste as hipóteses: Aplique os testes estatísticos aos dados para avaliar se as hipóteses são suportadas ou refutadas. Os resultados dos testes ajudarão a tomar decisões informadas.

- Interprete os resultados: Analise os resultados dos testes estatísticos e interprete o que eles significam em relação às hipóteses formuladas. Isso pode levar a novas questões ou direcionar sua análise de maneira diferente.

- Comunique as descobertas: Finalmente, comunique suas descobertas de forma clara e objetiva, destacando as hipóteses confirmadas ou refutadas, e suas implicações no contexto do problema ou questão original.

Lembrando que a análise exploratória de dados é um processo iterativo, e as hipóteses podem ser ajustadas à medida que você obtém mais informações e insights do conjunto de dados.

> retornar ao [**sumário**](#sumário).
>
> [voltar](./notes.md) para página anterior.
