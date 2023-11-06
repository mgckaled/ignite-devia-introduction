# Módulo 3 - Estatística para Devs

> [voltar](./notes.md) para página anterior.

## Sumário

- [Módulo 3 - Estatística para Devs](#módulo-3---estatística-para-devs)
  - [Sumário](#sumário)
  - [Conceitos](#conceitos)
    - [Estatística Descritiva](#estatística-descritiva)
    - [Medidas de Posição](#medidas-de-posição)
    - [Medidas de Dispersão](#medidas-de-dispersão)
    - [Medidas de Forma](#medidas-de-forma)
    - [Correlação](#correlação)

O objetivo deste módulo é apresentar os principais conceitos de [Estatística Descritiva](#estatística-descritiva), para uso em análise de dados

## Conceitos

### Estatística Descritiva

A Estatística Descritiva, quando vista dentro do contexto da Inteligência Artificial (IA), refere-se a uma abordagem estatística que é frequentemente usada para analisar e resumir dados em conjuntos de dados grandes e complexos. A IA desempenha um papel importante na análise e interpretação de dados, e a Estatística Descritiva é uma das técnicas fundamentais usadas para entender as características dos dados e extrair informações relevantes.

A Estatística Descritiva envolve o uso de várias medidas estatísticas para descrever e resumir um conjunto de dados. Alguns dos conceitos e técnicas da Estatística Descritiva incluem:

1. Medidas de tendência central: Isso inclui a média (média aritmética), a mediana (valor central) e a moda (valor mais frequente). A IA pode ser usada para calcular essas medidas rapidamente em grandes volumes de dados.

2. Medidas de dispersão: Isso envolve calcular a variância, o desvio padrão e a amplitude dos dados para entender o quão dispersos eles estão em relação à média. A IA pode automatizar o cálculo dessas medidas em grandes conjuntos de dados.

3. Gráficos e visualizações: A IA pode gerar gráficos e visualizações interativas para representar os dados de maneira mais compreensível. Isso pode incluir histogramas, gráficos de dispersão, box plots e muito mais.

4. Tabelas de frequência: A IA pode criar tabelas de frequência para resumir a distribuição de valores em um conjunto de dados, tornando mais fácil identificar padrões e tendências.

5. Análise de outliers: A IA pode identificar automaticamente valores atípicos (outliers) em conjuntos de dados, o que é importante para detectar erros de medição ou dados anômalos.

6. Resumo estatístico: A IA pode gerar um resumo estatístico completo de um conjunto de dados, incluindo todas as medidas descritivas relevantes.

Dentro da IA, a Estatística Descritiva é uma etapa fundamental no processo de análise de dados. Ela ajuda a compreender a distribuição dos dados, identificar tendências, anomalias e padrões, e permite que os cientistas de dados e engenheiros de IA tomem decisões informadas sobre como processar e modelar esses dados para construir modelos de aprendizado de máquina ou tomar outras ações com base nas informações extraídas.

> [voltar](#sumário) para o topo da página.

### Medidas de Posição

Medidas de posição são estatísticas descritivas usadas para resumir ou descrever a localização típica de um conjunto de dados em um contexto estatístico. Elas ajudam a entender onde os valores estão concentrados e a identificar valores atípicos ou extremos em um conjunto de dados. As medidas de posição mais comuns incluem a média, a mediana, a moda, o quartil e o percentil. Aqui estão algumas informações sobre cada uma delas:

1. **Média**: A média, também conhecida como média aritmética, é a soma de todos os valores em um conjunto de dados dividida pelo número de observações. É uma medida que fornece o valor médio dos dados. A média é sensível a valores extremos, também chamados de outliers.

2. **Mediana**: A mediana é o valor que divide um conjunto de dados em duas metades iguais, ou seja, metade dos valores está acima da mediana e metade está abaixo. A mediana é menos afetada por valores extremos do que a média e é especialmente útil quando os dados têm outliers.

3. **Moda**: A moda é o valor que ocorre com mais frequência em um conjunto de dados. Pode haver uma moda (unimodal) ou mais de uma moda (multimodal) em um conjunto de dados. A moda é especialmente útil para dados categóricos ou discretos.

4. **Quartis**: Os quartis dividem um conjunto de dados ordenado em quatro partes iguais. O primeiro quartil (Q1) é o valor abaixo do qual está o primeiro quartil dos dados. O segundo quartil (Q2) é a mediana, e o terceiro quartil (Q3) é o valor abaixo do qual está o terceiro quartil dos dados. Os quartis são úteis para entender a dispersão dos dados e identificar valores extremos.

5. **Percentis**: Os percentis dividem um conjunto de dados em 100 partes iguais. O p-ésimo percentil é o valor abaixo do qual está o p-ésimo percentil dos dados. O percentil 50 é a mediana. Os percentis são úteis para entender como os valores se distribuem em relação a uma escala percentual.

Além dessas medidas, também existem outros conceitos relacionados, como a média ponderada, a média geométrica, a média harmônica e outros percentis específicos, como o 25º e o 75º percentis, que são frequentemente usados em análises estatísticas.

A escolha da medida de posição apropriada depende do tipo de dados e do objetivo da análise estatística. Em muitos casos, é útil usar várias medidas de posição em conjunto para obter uma compreensão mais completa da distribuição dos dados.

> [voltar](#sumário) para o topo da página.

### Medidas de Dispersão

As medidas de dispersão são estatísticas descritivas que indicam a extensão ou a propagação dos dados em um conjunto. Elas são fundamentais para entender a variabilidade dos dados e quão distantes os valores estão da medida central (como a média, mediana ou moda). As principais medidas de dispersão incluem a amplitude, a variância, o desvio padrão, o intervalo interquartil e o coeficiente de variação. Vamos explorar cada uma delas:

1. **Amplitude**: A amplitude é a diferença entre o maior e o menor valor em um conjunto de dados. É uma medida simples de dispersão, mas é sensível a valores extremos e pode não ser representativa da verdadeira distribuição dos dados em conjuntos grandes ou com outliers.

2. **Variância**: A variância mede o quão distantes os valores estão da média. É calculada pela média dos quadrados das diferenças entre cada valor e a média do conjunto de dados. Valores mais altos de variância indicam uma dispersão maior dos dados.

3. **Desvio Padrão**: O desvio padrão é a raiz quadrada da variância e expressa a dispersão dos dados na mesma unidade que os dados originais. É uma medida amplamente utilizada, pois é mais interpretável do que a variância. Um desvio padrão maior indica maior dispersão dos dados.

4. **Intervalo Interquartil (IQR)**: O IQR é a diferença entre o terceiro quartil (Q3) e o primeiro quartil (Q1). Ele é menos sensível a valores extremos do que a amplitude, pois se baseia na distribuição dos quartis. O IQR é útil para identificar a dispersão dos dados no meio, ignorando os extremos.

5. **Coeficiente de Variação**: O coeficiente de variação (CV) é uma medida relativa de dispersão que expressa a variabilidade em termos de uma porcentagem da média. É útil para comparar a dispersão entre conjuntos de dados com escalas diferentes. Quanto menor o CV, mais homogêneo é o conjunto de dados.

É importante escolher a medida de dispersão apropriada com base na natureza dos dados e nos objetivos da análise. Por exemplo, se a presença de valores extremos é uma preocupação, o intervalo interquartil ou o desvio padrão podem ser mais indicados. Se a interpretabilidade é importante, o desvio padrão é frequentemente preferido. Compreender a dispersão dos dados é crucial para tomar decisões informadas e interpretar corretamente os resultados das análises estatísticas.

> [voltar](#sumário) para o topo da página.

### Medidas de Forma

Medidas de forma, também conhecidas como medidas de assimetria e curtose, são estatísticas descritivas que ajudam a caracterizar a forma da distribuição de dados em um conjunto. Essas medidas são importantes para compreender a simetria, a achatamento e outras características da distribuição dos dados. As duas principais medidas de forma são a assimetria (skewness) e a curtose (kurtosis):

1. **Assimetria (Skewness)**: A assimetria descreve a inclinação ou a assimetria da distribuição dos dados em relação à sua média. Ela pode ser positiva, negativa ou zero.

   - Assimetria positiva (skewness > 0): A cauda direita da distribuição é mais longa, e a maioria dos valores está concentrada na parte esquerda da distribuição.

   - Assimetria negativa (skewness < 0): A cauda esquerda da distribuição é mais longa, e a maioria dos valores está concentrada na parte direita da distribuição.

   - Assimetria zero (skewness = 0): A distribuição é simétrica, com valores igualmente distribuídos em ambos os lados da média.

   A medida de assimetria pode ajudar a identificar se uma distribuição é simétrica ou se está inclinada para um dos lados.

2. **Curtose (Kurtosis)**: A curtose indica o grau de achatamento ou apontamento da distribuição de dados em relação à distribuição normal (distribuição com curtose zero). Ela pode ser positiva (leptocúrtica), negativa (platicúrtica) ou zero (mesocúrtica).

   - Curtose positiva (kurtosis > 0): A distribuição possui caudas mais pesadas e é mais pontiaguda no centro do que a distribuição normal. Isso indica a presença de valores extremos ou picos pronunciados na distribuição.

   - Curtose negativa (kurtosis < 0): A distribuição é mais achatada e dispersa em comparação com a distribuição normal. Isso sugere que os valores estão menos concentrados no centro e têm caudas mais leves.

   - Curtose zero (kurtosis = 0): A distribuição possui a mesma achatamento da distribuição normal. É uma distribuição mesocúrtica.

   A medida de curtose ajuda a avaliar a forma da distribuição e a identificar se ela é mais ou menos "afilada" do que a distribuição normal.

É importante observar que a interpretação das medidas de forma depende do contexto dos dados e das características específicas da distribuição. Além disso, essas medidas não são as únicas considerações ao analisar a forma de uma distribuição; a visualização dos dados por meio de gráficos, como histogramas e gráficos de densidade, também é fundamental para uma compreensão completa da distribuição dos dados. As medidas de forma são ferramentas úteis para resumir a forma das distribuições, mas devem ser usadas em conjunto com outras técnicas de análise de dados.

> [voltar](#sumário) para o topo da página.

### Correlação

A correlação é uma medida estatística que descreve a relação entre duas variáveis em um conjunto de dados. Ela avalia o grau de associação ou dependência entre essas variáveis. A correlação é amplamente usada na estatística para entender como duas variáveis se comportam em conjunto e se há alguma relação linear entre elas. As principais medidas de correlação incluem o coeficiente de correlação de Pearson, o coeficiente de correlação de Spearman e o coeficiente de correlação de Kendall:

1. **Coeficiente de Correlação de Pearson (r)**: Este é o método mais comum para calcular a correlação entre duas variáveis quantitativas. O coeficiente de Pearson mede a força e a direção da relação linear entre as variáveis. Ele varia de -1 a 1, onde:

   - 1 indica uma correlação positiva perfeita, significando que as variáveis aumentam juntas de forma linear.
   - -1 indica uma correlação negativa perfeita, significando que as variáveis diminuem juntas de forma linear.
   - 0 indica que não há correlação linear entre as variáveis.

   No entanto, é importante observar que o coeficiente de Pearson avalia apenas relações lineares e pode não capturar relações não lineares.

2. **Coeficiente de Correlação de Spearman**: O coeficiente de Spearman é usado quando as variáveis não têm uma relação linear, mas ainda existe uma relação monotônica entre elas. Ele é calculado com base nas classificações das variáveis, tornando-o robusto a outliers e adequado para dados ordinais ou não normalmente distribuídos.

3. **Coeficiente de Correlação de Kendall (Tau)**: Assim como o coeficiente de Spearman, o coeficiente de Kendall também é usado para medir a correlação entre variáveis quando a relação não é linear e quando os dados são ordinais ou não normalmente distribuídos. Ele se baseia na contagem de pares concordantes e discordantes nas classificações das variáveis.

A correlação não implica causalidade. Ou seja, mesmo que duas variáveis estejam correlacionadas, não significa que uma cause a outra. Pode haver outras variáveis ocultas ou fatores de confusão que expliquem a relação.

Além disso, é importante lembrar que a correlação é sensível a valores extremos (outliers). Um ou mais outliers podem distorcer significativamente a medida de correlação, mesmo que a relação entre as variáveis seja fraca.

A escolha do coeficiente de correlação apropriado depende das características dos dados e dos objetivos da análise. Em geral, a correlação é uma ferramenta valiosa para explorar e quantificar a relação entre variáveis, o que pode ser útil em pesquisas científicas, análises de mercado, previsões e muitos outros campos.

> [voltar](#sumário) para o topo da página.
>
> [voltar](./notes.md) para página anterior.
