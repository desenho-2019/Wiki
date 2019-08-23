# Wiki

## Instalação
    - sudo apt install mkdocs
    ou
    - pip install mkdocs

## Inicializando o servidor local
    - mkdocs serve
    - Abra o seu navegador e digite a seguinte URL http://localhost:8000/

## Editando paginas
    - site_name: My Docs
      nav:
          - Home: index.md
          - About: about.md

## Gerando os arquivos estáticos
    - mkdocs build

## Deploy para o GitHub
    - mkdocs gh-deploy
