# Projeto Python com Docker e GitHub Actions

Este projeto foi desenvolvido para praticar conceitos de Python, Docker, testes automatizados e integração contínua (CI) utilizando GitHub Actions.

## Objetivo

O objetivo do projeto é executar uma aplicação Python dentro de um container Docker e realizar testes automatizados para verificar o funcionamento das funções desenvolvidas.

O projeto também utiliza o GitHub Actions para automatizar a execução dos testes quando um Pull Request é criado para a branch `main`.

## Tecnologias utilizadas

Python 3.10, Docker, GitHub Actions e Git.

## Estrutura do projeto

O projeto possui um arquivo `main.py`, responsável pela aplicação principal, um arquivo `test.py`, responsável pelos testes automatizados, um `Dockerfile`, utilizado para criar o container da aplicação, e um workflow do GitHub Actions localizado em `.github/workflows/test.yml`.

## Aplicação Python

O arquivo `main.py` contém uma função chamada `soma`, responsável por realizar a soma de dois valores. O arquivo também possui uma mensagem utilizada para verificar se a aplicação está sendo executada corretamente dentro do Docker.

## Testes automatizados

O arquivo `test.py` contém testes para verificar o funcionamento da função `soma`. São testadas diferentes situações, incluindo números positivos, números negativos, zero e combinações entre valores positivos e negativos.

## Docker

O projeto possui um `Dockerfile` baseado na imagem Python 3.10. O arquivo configura o diretório de trabalho, copia os arquivos do projeto para o container e define o `main.py` como arquivo principal a ser executado.

Para criar a imagem Docker, pode ser utilizado o comando:

```bash
docker build -t projeto-python .
```

Para executar o container:

```bash
docker run projeto-python
```

## GitHub Actions

O projeto utiliza GitHub Actions para automatizar a execução dos testes. O workflow está configurado para ser executado quando um Pull Request é criado para a branch `main`.

Durante a execução, o GitHub Actions acessa o código do repositório e executa o arquivo `test.py`, permitindo verificar automaticamente se os testes foram aprovados.

## Conceitos praticados

Este projeto permitiu praticar conceitos de desenvolvimento em Python, testes automatizados, utilização de containers com Docker, controle de versão com Git e GitHub e automação de testes utilizando GitHub Actions e integração contínua.

## Autora

Anna Prado

Projeto desenvolvido para fins acadêmicos e de aprendizado.
