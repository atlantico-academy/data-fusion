# Data Fusion 

Este projeto realiza uma análise abrangente dos dados de carros de 1970 a 2024. Utilizando um dataset do Kaggle, exploramos tendências, características e outras informações relevantes sobre os veículos ao longo dos anos. Esta análise pode ajudar em estudos de mercado, desenvolvimento de novos produtos e estratégias de marketing.

## Desenvolvedores

- Sarah Almeida Dalla Valle Prior #1
- João Vinicius Araújo Rocha #2
- Kassia Cristina de Sousa Lopes #3
- Alesangela Bezerra da Fonseca #4

## Funcionalidades

Esse template foi inicialmente baseado no template de ciência de dados do cookiecutter, mas ao longo do tempo várias modificações foram sendo realizadas. Atualmente o template tem as seguintes características:

- Utilização do arquivo `pyproject.toml` como centralizador de dependências;
- Configuração para criação de aplicação Streamlit;
- Utilização de Jupyter Notebooks para análise de dados;
- Documentação com o MkDocs (Material Design Theme).

## Instruções

### Requisitos

Para utilizar este template, você precisará de um ambiente com os seguintes softwares:

- `git`
- Python 3.8
- Poetry 1.1.13 ou superior

É aconselhável o uso do `pyenv` para o gerenciamento de versões do Python.

### Iniciando um novo projeto

Para iniciar um novo projeto a partir deste template:

1. Clicar no botão **"Use this template"** (ou "Usar este modelo").
2. Digitar um nome para seu repositório e uma descrição opcional.
3. Escolher a visibilidade do projeto (Pública ou privada).
4. Clicar em **"Create repository from template"** (Criar repositório a partir do modelo).

### Contribuindo com um repositório já criado

Para clonar o repositório e começar a contribuir:

1. Acima da lista de arquivos, clique no botão **"Code"** (em verde).
2. Copie a URL do repositório.
3. Utilize uma chave SSH para clonar:
    ```bash
    git clone git@github.com:NOME-DE-USUARIO/REPOSITORIO.git
    ```
4. Navegue até o diretório do repositório clonado:
    ```bash
    cd REPOSITORIO
    ```
5. Instale as dependências do projeto:
    ```bash
    poetry install
    ```
6. Ative o ambiente virtual criado pelo Poetry:
    ```bash
    poetry shell
    ```

## Utilização

Após a instalação, você pode iniciar a aplicação Streamlit para visualizar a análise dos dados:

```bash
streamlit run app.py
```

Ou abrir e executar os Jupyter Notebooks para explorar as análises de dados:

```bash
jupyter notebook notebooks/
```

## Organização de Diretórios

```plaintext
.
├── data/              # Diretório contendo todos os arquivos de dados
│   ├── external/      # Arquivos de dados de fontes externas
│   ├── interim/       # Arquivos de dados intermediários
│   ├── processed/     # Arquivos de dados processados
│   └── raw/           # Arquivos de dados originais, imutáveis
├── docs/              # Documentação gerada através da biblioteca MkDocs
├── models/            # Modelos treinados e serializados, predições ou resumos de modelos
├── notebooks/         # Diretório contendo todos os notebooks utilizados nos passos
├── references/        # Dicionários de dados, manuais e todo o material exploratório
├── src/               # Código fonte utilizado nesse projeto
│   ├── data/          # Classes e funções utilizadas para download e processamento de dados
│   ├── deployment/    # Classes e funções utilizadas para implantação do modelo
│   └── model/         # Classes e funções utilizadas para modelagem
├── app.py             # Arquivo com o código da aplicação do Streamlit
├── Procfile           # Arquivo de configuração do Heroku
├── pyproject.toml     # Arquivo de dependências para reprodução do projeto
├── poetry.lock        # Arquivo com sub-dependências do projeto principal
├── README.md          # Informações gerais do projeto
└── tasks.py           # Arquivo com funções para criação de tarefas utilizadas pelo invoke
```
