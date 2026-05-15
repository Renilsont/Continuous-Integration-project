# ANSWERS

## 1. Explique como a pipeline é disparada no GitHub Actions

A pipeline é disparada automaticamente quando ocorre um push na branch main.

Isso foi configurado no arquivo ci.yml através de:

```yaml
on:
  push:
    branches:
      - main

## 2. O que é um runner no GitHub Actions e qual o seu papel na execução da pipeline?

O runner é a maquina responsável por executar os comandos definidos na pipeline.
Neste trabalho foi utilizado runs-on: ubuntu-latest, o github fornece uma máquina ubuntu parqa executar os passos da pipeline.

## 3. Qual a diferença entre buildar a aplicação inteira como binário e buildar a imagem Docker?

Ao buildar a aplicação apenas o executável do programa é gerado, já buildar uma imagem Docker cria um ambiente completo.

## 4. Por que usar Docker em uma pipeline CI pode ser útil?

Para padronização do ambiente e porque o docker evita problemas de dependências dferentes entre máquinas.
 