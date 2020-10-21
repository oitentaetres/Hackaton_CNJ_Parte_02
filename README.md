<p align="center">
  <img src="imagens/logo-cnj.jpg" alt="Unform" />
</p>

<h3 align="center">
  HACKATHON CNJ 2020 🚀
</h3>

## Overview

As etapas presentes nesse repositório consolidam as Matrizes de Movimentos Predecessores, geradas nas etapas anteriores (disponíveis em https://github.com/oitentaetres/Hackaton_CNJ_Parte_01 ), na forma da Matriz de Contagem, que registra quantas ocorrências de cada movimento anterior estão associadas a cada um dos movimentos inseridos. Para isso, os arquivos MatrizPredecessor*.csv devem ser reunidos numa mesma pasta, como está exemplificado nesse repositório, e devem ser executados os notebooks relativos às etapas 05 e 06.

A Matriz de Contagem é gerada com a execução da Etapa 05. Em seguida, com a execuçaõ da Etapa 06, essa Matriz de Contagem é utilizada para gerar a Matriz de Padrões, que identifica os seis movimentos anteriores mais comuns em relação a cada um dos movimentos inseridos. Dessa forma, através dessa abordagem de "cesta de compras", podem ser identificado os movimentos mais comuns, sendo que os demais são interpretados como "red flags".

Como "output" das etapas 05 e 06, são gerados os seguintes arquivos:

  - matrizContagem.csv
  - matrizPadrao.csv
  - matrizPadrao.json
  
Os arquivos matrizPadrao.csv e matrizPadrao.json possibilitam que o conehcimento obtido nessa etapa seja utilizado na implementação da UI. Nesse caso, quando o servidor vai cadastrar um novo movimento no sistema, é verificado se o movimento anterior está de acordo com o padrão identificado. Em caso negativo, é gerado um alerta solicitando que o servidor verifique se o movimento cadastrado realmente é aquele ou se houve algum erro. Cabe ressaltar que nem todos os cadastramentos identificados como divergentes do padrão serão necessariamente erros, devido às especificidades de cada processo judicial.

## Installation

A linguagem de programção utilizada nesse desenvolvimento foi o Python, por isso caso não possua instalado, pode instalar nesse link: https://www.python.org/downloads/ .

Recomendo instalar também o Anaconda, que possui o ambiente Jupyter Notebook, que foi utilizado no desenvolvimento. Download nesse link: https://www.anaconda.com/products/individual .

Para instalar as bibliotecas python utilizadas, em um console, utilize o comando "pip".

Exemplo:

```
>>> pip install -U spacy
```

Lista de bibliotecas utilizadas nessas etapas:

  - pip install -U pandas
  - pip install -U glob
