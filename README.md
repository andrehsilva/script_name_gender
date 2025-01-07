
# Identificação de Gênero a partir de Nomes

Este projeto tem como objetivo identificar o gênero de pessoas com base em seus primeiros nomes, utilizando a biblioteca `genderbr` para consultar o gênero mais comum de nomes no Brasil. O projeto também inclui a leitura e manipulação de um arquivo Excel, realizando o processamento e atualização das informações de gênero, além de gerar um novo arquivo Excel com os resultados.

## Tecnologias Utilizadas

-   **Python 3**
-   **Pandas**: Biblioteca para manipulação e análise de dados.
-   **genderbr**: Biblioteca para consulta de gênero baseado em nomes brasileiros.
-   **Colab**: Ambiente de desenvolvimento utilizado para execução do código.
-   **Excel (xlsx)**: Formato de arquivo utilizado para importar e exportar dados.

## Funcionalidades

-   Leitura de um arquivo Excel contendo uma lista de nomes.
-   Extração do primeiro nome de cada registro.
-   Identificação do gênero (masculino, feminino ou desconhecido) com base no primeiro nome.
-   Atualização do DataFrame com o gênero identificado e outros tratamentos relacionados.
-   Geração de um arquivo Excel com os resultados do processamento.

## Instalação e Uso

### 1. Instale as dependências

Antes de rodar o código, é necessário instalar a biblioteca `genderbr`. Caso esteja utilizando o Google Colab, você pode rodar o seguinte comando:

python

Copiar código

`!pip install genderbr` 

### 2. Preparação do Arquivo Excel

O arquivo Excel que será lido deve conter uma coluna chamada **"nome"** com os nomes completos. O código irá extrair o primeiro nome e utilizar essa informação para determinar o gênero.

### 3. Execução do Código

O código realiza os seguintes passos:

1.  Importação e instalação das dependências necessárias.
2.  Carregamento e leitura do arquivo Excel.
3.  Extração do primeiro nome de cada registro e consulta do gênero utilizando a função `get_gender`.
4.  Atualização da coluna **"genero"** no DataFrame com os valores "Masculino", "Feminino" ou "Desconhecido".
5.  Geração de um novo arquivo Excel com os resultados, incluindo a coluna "genero" e outras informações derivadas.

### 4. Saída

O arquivo resultante será salvo em um novo arquivo Excel com o nome **"name_gender_output.xlsx"**. O arquivo estará localizado no mesmo diretório de onde o script é executado.

## Exemplo de Uso

Para rodar o script, basta carregar o arquivo Excel com a lista de nomes e executar o código no ambiente Python (ou Google Colab). O processo de identificação de gênero será automaticamente realizado.

## Licença

Este projeto está sob a licença MIT - veja o arquivo LICENSE para mais detalhes.
