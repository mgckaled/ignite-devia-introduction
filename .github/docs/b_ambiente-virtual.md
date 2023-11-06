# Módulo 2 - Ambiente Virtual de Desenvolvimento

> [voltar](./notes.md) para página anterior.

## Sumário

- [Módulo 2 - Ambiente Virtual de Desenvolvimento](#módulo-2---ambiente-virtual-de-desenvolvimento)
  - [Sumário](#sumário)
  - [Objetivo do módulo](#objetivo-do-módulo)
  - [Conteúdo](#conteúdo)
    - [O que é Ambiente Virtual de desenvolvimento?](#o-que-é-ambiente-virtual-de-desenvolvimento)
    - [Quais são os principais gerenciadores de versão Python?](#quais-são-os-principais-gerenciadores-de-versão-python)
    - [O que é e qual é o objetivo dos Gerenciadores de Ambientes Virtuais?](#o-que-é-e-qual-é-o-objetivo-dos-gerenciadores-de-ambientes-virtuais)
    - [Gerenciadores de Ambiente Virtual minimalistas](#gerenciadores-de-ambiente-virtual-minimalistas)
      - [`Pyenv`](#pyenv)
      - [`Pipenv`](#pipenv)

## Objetivo do módulo

Preparar adequadamente o ambiente de desenvolvimento para as tarefas práticas do módulo.

## Conteúdo

### O que é Ambiente Virtual de desenvolvimento?

Um Ambiente Virtual de Desenvolvimento em Python é um espaço isolado que permite criar um ambiente independente com suas próprias configurações e dependências Python para um projeto específico. Isso ajuda a evitar conflitos entre bibliotecas e permite que os desenvolvedores gerenciem diferentes conjuntos de bibliotecas e versões para diferentes projetos Python em uma única máquina.

### Quais são os principais gerenciadores de versão Python?

Os principais gerenciadores de versão Python são:

1. **pip**: O pip é o gerenciador de pacotes padrão do Python. Ele é usado para instalar, atualizar e remover pacotes Python do Python Package Index (PyPI) e de outros repositórios.

2. **virtualenv**: O virtualenv é uma ferramenta que permite criar ambientes virtuais isolados para seus projetos Python. Isso ajuda a evitar conflitos entre dependências e a manter diferentes ambientes Python para diferentes projetos.

3. **venv**: O venv é um módulo Python incorporado a partir da versão 3.3 que oferece funcionalidades semelhantes ao virtualenv para criar ambientes virtuais isolados. É uma alternativa mais recente e integrada ao Python.

4. **conda (Conda Environment)**: Conda é uma ferramenta de gerenciamento de pacotes e ambientes que não é específica para Python, mas é amplamente usada na comunidade de ciência de dados e aprendizado de máquina. Ela permite criar ambientes virtuais independentes e gerenciar pacotes Python e não Python.

5. **pyenv**: O pyenv é um utilitário que permite gerenciar múltiplas instalações do interpretador Python na mesma máquina. Isso facilita a alternância entre diferentes versões do Python em diferentes projetos.

6. **poetry**: O poetry é uma ferramenta que visa simplificar o gerenciamento de dependências e a criação de ambientes virtuais para projetos Python. Ele combina gerenciamento de pacotes e criação de ambientes virtuais em uma única ferramenta.

7. **pipenv**: O pipenv é outra ferramenta que visa simplificar o gerenciamento de dependências e ambientes virtuais Python. Ele combina o uso do pip para instalação de pacotes com um arquivo Pipfile para gerenciar dependências e um ambiente virtual criado automaticamente.

8. **Anaconda**: O Anaconda é uma distribuição de código aberto que inclui o Conda e muitas bibliotecas científicas e de análise de dados. Ele é amplamente utilizado em ciência de dados e aprendizado de máquina.

A escolha do gerenciador de versão Python depende das necessidades e preferências do desenvolvedor, bem como das exigências do projeto. Cada um desses gerenciadores oferece recursos específicos e aborda diferentes aspectos do desenvolvimento e do gerenciamento de pacotes Python.

> [voltar](#sumário) para o topo da página.

### O que é e qual é o objetivo dos Gerenciadores de Ambientes Virtuais?

Os Gerenciadores de Ambientes Virtuais são ferramentas que permitem criar e gerenciar ambientes de desenvolvimento isolados para projetos de software. O objetivo principal desses gerenciadores é isolar e controlar as dependências e configurações específicas de cada projeto, garantindo que diferentes projetos não entrem em conflito uns com os outros. Aqui está uma explicação mais detalhada:

1. **Isolamento de Ambiente**:
   - O principal objetivo é isolar o ambiente de desenvolvimento de um projeto do sistema global do computador. Cada ambiente virtual possui sua própria cópia do interpretador Python e suas próprias bibliotecas e dependências.
   - Isso ajuda a evitar conflitos entre diferentes versões de bibliotecas Python que podem ser necessárias para diferentes projetos. Por exemplo, um projeto pode exigir a versão 1.0 de uma biblioteca, enquanto outro projeto precisa da versão 2.0. Ambientes virtuais garantem que essas versões não interfiram umas com as outras.

2. **Gerenciamento de Dependências**:
   - Os gerenciadores de ambientes virtuais também facilitam o controle e a instalação de dependências específicas de um projeto. Você pode listar todas as bibliotecas necessárias para um projeto em um arquivo de requisitos e, em seguida, usar o gerenciador para instalá-las automaticamente no ambiente virtual.
   - Isso torna mais fácil para os desenvolvedores compartilhar e replicar ambientes de desenvolvimento consistentes.

3. **Portabilidade e Colaboração**:
   - Os ambientes virtuais tornam os projetos mais portáteis, pois você pode compartilhar facilmente o ambiente virtual (juntamente com o arquivo de requisitos) com outros desenvolvedores. Isso permite que outros desenvolvedores reproduzam facilmente o ambiente de desenvolvimento em suas próprias máquinas.
   - Facilitam a colaboração em equipe, pois os membros da equipe podem trabalhar em ambientes virtuais idênticos, garantindo consistência no desenvolvimento.

4. **Versões do Python**:
   - Os gerenciadores de ambientes virtuais também permitem que você trabalhe com diferentes versões do Python em diferentes projetos. Isso é útil quando você precisa migrar gradualmente seus projetos para uma nova versão do Python, pois cada ambiente virtual pode ser configurado para uma versão específica do Python.

Em resumo, os gerenciadores de ambientes virtuais são ferramentas essenciais para o desenvolvimento Python, pois ajudam a criar ambientes de desenvolvimento isolados, controlar dependências e garantir a consistência e a portabilidade de projetos. Eles desempenham um papel fundamental na organização e na simplificação do gerenciamento de projetos de software.

> [voltar](#sumário) para o topo da página.

### Gerenciadores de Ambiente Virtual minimalistas

#### `Pyenv`

O `pyenv` é uma ferramenta que permite gerenciar múltiplas instalações do interpretador Python em uma única máquina. Ela oferece flexibilidade para alternar entre diferentes versões do Python e é útil quando você precisa trabalhar com projetos que requerem versões específicas do Python. Abaixo, vou fornecer explicações detalhadas sobre o `pyenv`:

**Instalação do Pyenv:**

Para começar a usar o `pyenv`, você precisa instalá-lo em seu sistema. O processo de instalação pode variar dependendo do seu sistema operacional. Geralmente, você pode instalar o `pyenv` seguindo as instruções no GitHub do projeto (<https://github.com/pyenv/pyenv>).

**Uso Básico do Pyenv:**

Aqui estão alguns comandos e conceitos importantes relacionados ao `pyenv`:

1. **Listar Versões Disponíveis:**
   - Você pode listar todas as versões do Python disponíveis para instalação usando o comando:

     ```shell
     pyenv install --list
     ```

2. **Instalar Versões do Python:**
   - Para instalar uma versão específica do Python, você pode usar o comando:

     ```shell
     pyenv install <versão>
     ```

   - Por exemplo, para instalar o Python 3.8.12:

     ```shell
     pyenv install 3.8.12
     ```

3. **Definir uma Versão Global:**
   - Você pode definir uma versão global do Python para todo o seu sistema usando:

     ```shell
     pyenv global <versão>
     ```

   - Isso afetará todos os projetos que não têm uma versão específica definida localmente.

4. **Definir uma Versão Local:**
   - Em um projeto específico, você pode definir uma versão local do Python usando:

     ```shell
     pyenv local <versão>
     ```

   - Isso criará um arquivo `.python-version` no diretório do projeto para indicar qual versão deve ser usada quando você entrar naquele diretório.

5. **Listar Versões Disponíveis e Atual:**
   - Para listar todas as versões Python instaladas e indicar qual está atualmente em uso, você pode usar:

     ```shell
     pyenv versions
     ```

6. **Alternar Entre Versões:**
   - Você pode alternar entre diferentes versões do Python usando o comando `pyenv global`, `pyenv local` ou mesmo definindo a variável de ambiente `PYENV_VERSION`.

**Vantagens do Pyenv:**

- **Flexibilidade**: O `pyenv` permite que você trabalhe com várias versões do Python no mesmo sistema, tornando-o flexível para lidar com projetos que têm diferentes requisitos de versão.

- **Isolamento**: Ele não cria ambientes virtuais como o `virtualenv` ou `venv`, mas oferece uma maneira de isolar diferentes instalações do Python, evitando conflitos de dependências entre projetos.

- **Portabilidade**: Você pode compartilhar seu arquivo `.python-version` com outros membros da equipe, permitindo que todos usem a mesma versão do Python para um projeto específico.

- **Fácil Alternância**: Alternar entre diferentes versões do Python é simples e pode ser feito globalmente ou em nível de projeto.

- **Suporte à Comunidade**: O `pyenv` é uma ferramenta amplamente usada e suportada pela comunidade Python, com uma grande base de usuários e contribuidores.

Em resumo, o `pyenv` é uma ferramenta valiosa para gerenciar versões do Python em seu sistema, tornando-o especialmente útil quando você precisa trabalhar com projetos que têm diferentes requisitos de versão do Python. Ele ajuda a manter o controle e a flexibilidade em seu ambiente de desenvolvimento Python.

#### `Pipenv`

O `pipenv` é uma ferramenta de gerenciamento de pacotes e ambientes virtuais Python que visa simplificar o processo de desenvolvimento, gerenciando dependências e ambientes virtuais. Ele combina as funcionalidades do `pip` (gerenciador de pacotes) e do `virtualenv` (gerenciador de ambientes virtuais) em uma única ferramenta. Abaixo, vou fornecer explicações detalhadas sobre o `pipenv`:

**Instalação do Pipenv:**

Para começar a usar o `pipenv`, você precisa instalá-lo em seu sistema. Você pode fazê-lo usando o `pip`, o gerenciador de pacotes Python padrão:

```shell
pip install pipenv
```

**Uso Básico do Pipenv:**

Aqui estão os conceitos e comandos importantes relacionados ao `pipenv`:

1. **Criar um Novo Ambiente Virtual e Inicializar um Projeto:**
   - Para criar um novo ambiente virtual e iniciar um projeto Python em um diretório específico, você pode usar:

     ```shell
     pipenv --python <versão do Python>
     ```

   - Isso criará um ambiente virtual e um arquivo `Pipfile` no diretório.

2. **Instalar Dependências:**
   - Você pode instalar dependências usando o `pipenv` da seguinte maneira:

     ```shell
     pipenv install <pacote>
     ```

   - Isso instala o pacote especificado no ambiente virtual e o adiciona ao arquivo `Pipfile`.

3. **Ativar o Ambiente Virtual:**
   - Para ativar o ambiente virtual, você pode usar:

     ```shell
     pipenv shell
     ```

   - Isso permite que você trabalhe dentro do ambiente virtual, onde as dependências específicas do projeto são usadas.

4. **Desativar o Ambiente Virtual:**
   - Para sair do ambiente virtual e retornar ao ambiente global do sistema, você pode usar:

     ```shell
     exit
     ```

5. **Listar Dependências do Projeto:**
   - Para listar todas as dependências instaladas para o projeto atual, você pode usar:

     ```shell
     pipenv lock -r
     ```

6. **Remover Dependências Não Utilizadas:**
   - Você pode remover dependências não utilizadas com o comando:

     ```shell
     pipenv clean
     ```

7. **Gerar um Arquivo Lock (Pipfile.lock):**
   - O `pipenv` cria um arquivo `Pipfile.lock` que registra as versões exatas das dependências do projeto. Para gerá-lo, você pode usar:

     ```shell
     pipenv lock
     ```

**Vantagens do Pipenv:**

- **Integração de Gerenciamento de Pacotes e Ambientes Virtuais**: O `pipenv` combina o gerenciamento de pacotes (`pip`) e a criação de ambientes virtuais (`virtualenv`) em uma única ferramenta, simplificando o fluxo de trabalho de desenvolvimento.

- **Sintaxe Simples**: A sintaxe do `pipenv` é mais amigável e mais fácil de entender do que lidar com `requirements.txt` e `virtualenv` separadamente.

- **Reprodutibilidade**: O `Pipfile.lock` registra as versões exatas das dependências, tornando o ambiente de desenvolvimento altamente reprodutível e consistente.

- **Fácil Colaboração**: Com o `Pipfile` e `Pipfile.lock`, você pode compartilhar facilmente as informações sobre as dependências do projeto com outros membros da equipe.

- **Gerenciamento de Variáveis de Ambiente**: O `pipenv` também permite definir variáveis de ambiente específicas para o projeto no arquivo `Pipfile`.

- **Integração com Ferramentas Populares**: O `pipenv` é amplamente adotado pela comunidade Python e é bem integrado com outras ferramentas populares, como o Visual Studio Code e o PyCharm.

Em resumo, o `pipenv` é uma ferramenta conveniente e poderosa para gerenciamento de pacotes e ambientes virtuais em projetos Python. Ele oferece uma solução completa para criar ambientes de desenvolvimento isolados e gerenciar dependências, tornando o desenvolvimento Python mais organizado e eficiente.

> [voltar](#sumário) para o topo da página.
>
> [voltar](./notes.md) para página anterior.
