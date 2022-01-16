# Tech News :news_paper:

Este projeto foi desenvolvido durante o curso de desenvolvimento web da [Trybe](https://www.betrybe.com/).

### Descrição:
Aplicação em Python que faz raspagem das notícias de tecnologia no site do [TecMundo](https://www.tecmundo.com.br/novidades), formata e salva em um banco de dados Mongo.


### Principais tecnologias utilizadas:
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)

### Habilidades Desenvolvidas: 

- Utilizar o terminal interativo do Python;
- Escrever seus próprios módulos e importá-los em outros códigos;
- Aplicar técnicas de raspagem de dados;
- Extrair dados de conteúdo HTML;
- Armazenar os dados obtidos em um banco de dados.

### Como rodar a aplicação:

É necessário ter um servidor MongoDB rodando localmente, as instruções para instalar:
Ubuntu: https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/ 
MacOS: https://docs.mongodb.com/guides/server/install/

```bash
# Clone o repositório:
git clone https://github.com/Marcuscps19/python-job-insights.git

# Entre no diretório
cd python-job-insights

# Crie o ambiente virtual para o projeto
python3 -m venv .venv && source .venv/bin/activate

# Instale as dependências
python3 -m pip install -r dev-requirements.txt
```

No arquivo tech_news/menu.py, possui um menu de funcionalidades, para executá-o descomente o seguinte código no final do arquivo:

```
  if(__name__ == '__main__'):
    analyzer_menu()
```

#### Funcionalidades:

##### Popular o banco com notícias:
  Essa funcionalidade busca a quantidade de notícias digitada no site do TecMundo, e as salva no banco de dados.

##### Buscar notícias por título:
  Essa funcionalidade busca notícias por título no site do TecMundo  e as exibem no console, se não existir notícias com o título buscado retorna uma lista vazia.

##### Buscar notícias por data:
  Essa funcionalidade busca notícias por data no site do TecMundo  e as exibem no console, se não existir notícias com a data buscada retorna uma lista vazia.

##### Buscar notícias por fonte:
  Essa funcionalidade busca notícias pela fonte no site do TecMundo  e as exibem no console, se não existir notícias com a fonte buscada retorna uma lista vazia.

##### Buscar notícias por categoria:
  Essa funcionalidade busca notícias por categoria no site do TecMundo  e as exibem no console, se não existir notícias com a categoria buscada retorna uma lista vazia.

##### Listar top 5 notícias:
  Essa funcionalidade busca notícias no site do TecMundo e as classificam por popularidade(comentarios + compartilhamentos) e as exibem no console.

##### Listar top 5 categorias:
 Essa funcionalidade busca as 5 primeiras categorias do site do TecMundo, listando em ordem alfabética.
