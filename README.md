<!-- markdownlint-disable MD033 -->

# Formação Desenvovimento de IA - Introdução, Estatística e AED

<div align="center">
   <img alt="logo trilha" src=".github/assets/trilha-rs.png" width="40%"/>
</div>

<br>

<div align="center">
   <a href="https://github.com/mgckaled">
      <img alt="Made by mgckaled" src="https://img.shields.io/badge/made%20by-mgckaled-darkblue">
   </a>
   <img alt="GitHub Repo Size" src="https://img.shields.io/github/repo-size/mgckaled/ignite-devia-introduction">
   <img alt="GitHub Language Count" src="https://img.shields.io/github/languages/count/mgckaled/ignite-devia-introduction">
  <img alt="License" src="https://img.shields.io/static/v1?label=license&message=MIT&color=49AA26&labelColor=000000">
</div>

## Sumário

- [Formação Desenvovimento de IA - Introdução, Estatística e AED](#formação-desenvovimento-de-ia---introdução-estatística-e-aed)
  - [Sumário](#sumário)
  - [Sobre o Projeto](#sobre-o-projeto)
    - [Módulo 1: Introdução](#módulo-1-introdução)
    - [Módulo 2: Ambiente de Desenvolvimento](#módulo-2-ambiente-de-desenvolvimento)
    - [Módulo 3: Estatística para Devs](#módulo-3-estatística-para-devs)
    - [Módulo 4: Análise Exploratória de Dados com Pandas](#módulo-4-análise-exploratória-de-dados-com-pandas)
  - [Tecnologias](#tecnologias)
    - [Linguagem de Programação](#linguagem-de-programação)
    - [Gerenciadores de Ambiente Virtual](#gerenciadores-de-ambiente-virtual)
    - [Principais Bibliotecas (Packages)](#principais-bibliotecas-packages)
  - [Como clonar o projeto?](#como-clonar-o-projeto)
  - [Licença](#licença)

## Sobre o Projeto

Repositório que reuni os quatro primeiros módulos da formação Desenvolvimento IA 2023-2024, desenvolvido pela Rocketseat Education.

### Módulo 1: Introdução

Neste módulo de introdução à inteligência artificial, exploraremos conceitos e fundamentos da área, abordando seu potencial na resolução de problemas complexos. Também traçaremos uma linha do tempo desde suas origens históricas até o presente emocionante e o futuro promissor da IA, revelando seu impacto no mundo. Prepare-se para uma imersão profunda no universo da IA e sua influência na sociedade.

> Acesso ao [conteúdo das aulas](.github/docs/a_introducao.md) 

### Módulo 2: Ambiente de Desenvolvimento

Neste módulo de configuração para a formação de Desenvolvimento IA, focaremos em prepará-lo eficazmente para as tarefas práticas. Isso envolve entender ambientes virtuais, gerenciar versões do Python e configurar o Visual Studio Code. Exploraremos otimizações para interagir com Python na IA, maximizando sua experiência de aprendizado. Prepare-se para configurar seu ambiente de desenvolvimento de forma sólida, crucial para o sucesso na trilha de estudo.

> Acesso ao [conteúdo das aulas](.github/docs/b_ambiente-virtual.md)

### Módulo 3: Estatística para Devs

Neste módulo de Estatística Descritiva e Qualitativa para Devs, focaremos na construção de uma base sólida em conceitos-chave. Isso é essencial para analisar dados, explorar informações iniciais para insights valiosos e identificar padrões nos conjuntos de dados. Esses conhecimentos impactarão a escolha de modelos de machine learning, ajuste de parâmetros e avaliação de desempenho. Prepare-se para adquirir as habilidades essenciais para aplicar estatística descritiva com confiança em sua carreira na IA.

> Acesso ao [conteúdo das aulas](.github/docs/c_estatistica-devs.md). Respostas do questionário avaliativo ao final do documento.

- [Desafio opicional do módulo](https://efficient-sloth-d85.notion.site/Desafio-Estat-stica-para-Devs-f1fd60193670432b9ea6bab3e40c345c): `notebooks/challenge_m3.ipynb`

### Módulo 4: Análise Exploratória de Dados com Pandas

Neste módulo de análise exploratória de dados com pandas, vamos aprender a extrair insights dos dados que temos. O objetivo do EDA, ou Exploratory Data Analysis, é dar uma olhada nos dados antes de começar a fazer coisas mais complexas. Vamos abordar conceitos do EDA, a biblioteca Pandas, coleta e preparação de dados, lidar com dados ausentes, formulação de hipóteses, análise univariada e bivariada, lidar com outliers e automatizar parte do processo.

> Acesso ao [conteúdo das aulas](.github/docs/d_eda.md). Respostas do questionário avaliativo ao final do documento.

Ao final dos estudos, foi gerado um relatório automatizado na pasta `/reports`. 

- [Desafio opicional do módulo](https://efficient-sloth-d85.notion.site/Desafio-EDA-c8c8b2faf153449193b4b9fb0895afa6): `notebooks/challenge_m4.ipynb`

## Tecnologias

### Linguagem de Programação

- [`python`](https://www.python.org/) (v3.11.0)

### Gerenciadores de Ambiente Virtual

- [`pyenv`](https://github.com/pyenv/pyenv)
- [`pipenv`](https://pipenv.pypa.io/en/latest/)

### Principais Bibliotecas (Packages)

- [`pandas`](https://pandas.pydata.org/)
- [`matplotlib`](https://matplotlib.org/)
- [`scipy`](https://scipy.org/)
- [`numpy`](https://numpy.org/)
- [`sweetviz`](https://pypi.org/project/sweetviz/)

## Como clonar o projeto?

1. Certifique-se de que está usando o `pyenv` e o `pipenv` para gerenciar as dependências do projeto. Veja como instalar e configurar clicando nos respectivos links do tópico [Gerenciadores de Ambiente Virtual](#gerenciadores-de-ambiente-virtual).

2. Faça o clone pelo Github:

    ```bash
    git clone https://github.com/mgckaled/ignite-devia-introduction.git
    ```

3. Acesse o diretório:

    ```bash
    cd ignite-devia-introduction
    ```

4. Ative o ambiente virtual pelo terminal

    ```shell
    pipenv shell
    ```

5. Instale as dependências. (Certifique-se de estar utilzando a versão exata do python - 3.11.0)

    ```shell
    pipenv install
    ```

    ou, como um recurso de degurança, dependências exatas do `requirements.txt`:

    ```shell
    pipenv install -r requirements.txt
    ```

## Licença

Distribuído sob a licença *MIT*. Veja [LICENSE](LICENSE) para mais informações.

---

<h5 align="center">
  2023-2024 - <a href="https://github.com/mgckaled/">Marcel Kaled</a>
</h5>
