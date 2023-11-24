# PROJETO INDIVIDUAL 3 - Sistema RESILIADATA

## Descrição
Este projeto faz parte do Módulo 3 da Resilia, com o objetivo de modernizar o processo de armazenamento de dados e gerenciamento da estrutura de ensino da empresa.

## Conteúdo do Projeto
- [Contexto](#contexto)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Modelagem do Banco de Dados](#modelagem-do-banco-de-dados)
- [Relacionamentos](#relacionamentos)
- [Guia do Projeto](#guia-do-projeto)
- [Licença](#licença)
- [Status](#status)

## Contexto
O sistema visa auxiliar na avaliação de quais são as tecnologias que as empresas parceiras
estão utilizando e quem são seus colaboradores.


## Estrutura do Projeto
O projeto está estruturado da seguinte forma:
- `RESILIADATA.sql`: Contém o codigo para exução do banco de dados.
- `perguntas.txt`: Arquivo de texto contendo as respostas das questões.
- `modelo.png`: Print do modelo proposto

## Modelagem do Banco de Dados
### Entidades

1. empresa
    - id_empresa (INT, PK)
    - nome_empresa (VARCHAR(255))
    - endereco (VARCHAR(255))
    - telefone (VARCHAR(20))

2. tecnologias
    - id_tecnologias (INT, PK)
    - area (VARCHAR(50))
    - nome_tecnologia (VARCHAR(255))

3. tecnologia_empresa
    - id_empresa (INT, FK referenciando empresa)
    - id_tecnologias (INT, FK referenciando tecnologias)
    - nivel_utilizacao (INT)

4. colaborador
    - id_colaborador (INT, PK)
    - nome (VARCHAR(255))
    - cargo (VARCHAR(50))
    - id_empresa (INT, FK referenciando empresa)

## Relacionamentos

- Relacionamento 1:N entre empresa e colaborador (uma empresa pode ter vários colaboradores).
- Relacionamento N:N entre empresa e tecnologias através da tabela de associação Tecnologia_Empresa (uma empresa pode utilizar várias tecnologias, e uma tecnologia pode ser utilizada por várias empresas).


## Guia do Projeto
- [PDF com Instruções e Detalhes do Projeto](https://resilia-files-production.s3.amazonaws.com/material/student/1694009823_SEDadosM3ProjetoIndividualpdf.pdf?AWSAccessKeyId=ASIA5NG2YCRHBRI72THX&Expires=1700790780&Signature=S1USY69BT7rj2D8cT7hGYoDUrA8%3D&x-amz-security-token=IQoJb3JpZ2luX2VjEOz%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJIMEYCIQDpt1e%2BSVnBnOFVHT0o78lBu2%2FOJSZfNXcFnw6D%2BEzx4QIhAKFnDA5xOqi2gN9SdWksHJAHRwratBXmr53a5iuCQKJmKrMFCEUQAhoMOTIxNzI5MjQyMTkwIgz0V4KklshbHw9q8tAqkAWuznfqTn9s%2B%2FUbgNLYiLPpFqGJCyjH56s0BOnjr0ufo6SmYOfi8XIHNBSH0tFme8kKvTCJu2PAKUjOhIoOJL4VG5IWqQ2L%2BUzoWKtmS%2FOzOMq9f8sbfkd9yxjnWqzx7GZceyZtTeiEydBxEmDXr%2B%2BGVVNcE52IsooTtfOMx0xZfGp4IZfTnKrwzf%2ByBxm6pfBBJInAkPhCkmLJDQl63WLOFbFkev%2FcSUsk9mbPIy1XhcX4f6oq833u7b7XK6FGpRewj74hTPls0Z1vYlrIFxjgwvS1QhqAft3WEJ4rHlbNNSNxXX2hY98uQhX2kB1whpj5sUHKkBneQ7l4XEBBmiurSlGkMBUu2I7snBXzNkRGI7wgi15%2BJi85LvWltpfywL5JtTtv%2BA2QkQD4DV0f6BOOS6RyF%2BsJiEFSqAHcBTpdg0rFnS7b%2BiHFFBtGtlrdPQTF6hzAdlUQpoKQzp91iQ0N8Jlel1pLZDOb5jsophn1wBkDRcyUJvFRS8tTtvq4yWD7h6na656bFNo%2F04dyfpKlEpbZDYA8tZTV830EjkJpcCCTBVVfuZ4g50CyXHy0Bt9kmtRJ5IccZC3WMx%2BqNpH1sXnHGO338Y65aCUgMtNT3gT8RV7LLtHwzLKbvz0vpGWPIiqimmtHU%2Fxnuc0KnQzNHtqjk6%2BItMtBZPXGt%2BWlJxfdtZbOBJa0dgyV%2FarRsJ%2FD7MaOUcGau8e6KWtwWKiKKtbPNissLCCnO4uIajgDAXagwqONq%2F9BAxemXNI8bv%2F8lsZYLhXj%2BNRyqsmSsOecgZjxfF5DDwEPmE6TMVQvDL78tIh%2Fc6V4tdNPN%2BPUWIlpk%2B8JW1fmTPqaotzT5E4ForUeP1tUBrgMYUJ9v2%2FhtzCC%2FvyqBjqwAfLxFiwf4jl6ykFo7AK8VRS3Xcko3VGnjhbYceoOKimk%2FloQ7Wtotsz%2FMVBRMomU%2FFx4rJgRlurfogd9KOhleNMq9ihK6q16DfPQQ1GNJg%2FyeEFrPP9G1tmQqDI2Bcq1ot73YZVYrmVFWjzdQdWNd4OBepXlyrj8xudm1nba7S4XKCqxhbULCC9kbJlE4Qc7Cw2ocdmYbCoGO1k2hN0HQitQk71C%2B%2FL8rsCrRwOYPEm4)

## Licença

Este projeto é licenciado sob a [Licença MIT](LICENSE).



## Status
![GitHub Repo Size](https://img.shields.io/github/repo-size/NewKanvas/PI3?style=for-the-badge&logo=github)
![GitHub last commit](https://img.shields.io/github/last-commit/NewKanvas/PI3?style=for-the-badge&logo=git)
![Downloads](https://img.shields.io/github/downloads/NewKanvas/PI3/total?style=for-the-badge)
![Forks](https://img.shields.io/github/forks/NewKanvas/PI3.?style=for-the-badge)
![Watchers](https://img.shields.io/github/watchers/NewKanvas/PI3?style=for-the-badge)
![Stars](https://img.shields.io/github/stars/NewKanvas/PI3.?style=for-the-badge)
![Issues](https://img.shields.io/github/issues/NewKanvas/PI3.?style=for-the-badge)
