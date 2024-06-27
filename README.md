# 📚 Record Linkage Basics with Python

Este repositório contém scripts e dados utilizados para demonstrar a técnica de Record Linkage, aplicando Lógica Difusa (Fuzzy Logic) e o algoritmo de Levenshtein para comparar e unir registros de dois conjuntos de dados diferentes. A implementação é feita utilizando a linguagem Python e a biblioteca `recordlinkage`.

## 📂 Conteúdo

- **`notebook.ipynb`**: Notebook Jupyter com o código e as explicações detalhadas sobre cada passo da implementação do Record Linkage.
- **`book_release_year.csv`**: Conjunto de dados contendo informações sobre o ano de lançamento de livros.
- **`book_sold_copies.csv`**: Conjunto de dados contendo informações sobre a quantidade de cópias vendidas de livros.

## 🎯 Objetivo

O objetivo deste repositório é fornecer um exemplo claro e detalhado de como implementar a técnica de Record Linkage em Python. A técnica é fundamental para integrar dados de diferentes fontes, sendo amplamente utilizada em áreas como saúde, marketing e pesquisa.

## 🚀 Instruções de Uso

1. Clone este repositório:
    ```sh
    git clone https://github.com/<seu-usuario>/<nome-do-repositorio>.git
    ```

2. Instale as dependências necessárias:
    ```sh
    pip install pandas recordlinkage
    ```

3. Abra o notebook Jupyter:
    ```sh
    jupyter notebook notebook.ipynb
    ```

4. Siga as instruções e células no notebook para executar o exemplo de Record Linkage.

## 📋 Descrição dos Passos

1. **Carregar Conjuntos de Dados**: Utilizamos a biblioteca `pandas` para carregar e visualizar os dados dos arquivos CSV.
2. **Criação do Indexador**: Usamos o objeto `Index` da biblioteca `recordlinkage` para definir como os registros dos dois conjuntos de dados serão comparados.
3. **Criação do Objeto Comparar**: Configuramos o objeto `Compare` para definir os critérios de comparação entre os registros.
4. **Limpar o DataFrame Resultante**: Removemos colunas indesejadas do DataFrame resultante para uma análise mais clara dos dados comparados.

## 📊 Resultados

Vamos analisar os resultados. Observe que a ausência do apóstrofo (') nos títulos do conjunto B não impediu a correta associação das obras "The Hitchhiker's Guide to the Galaxy" e "Foundation's Edge". No entanto, a obra "The War of the Words" de Rachael Jolley foi erroneamente associada a "The War of the Worlds" de H. G. Wells. Nesse caso, a diferença na letra "l" foi significativa.

## ✅ Conclusão

A técnica de Record Linkage é uma ferramenta poderosa para integrar dados de diferentes fontes. Usando Python e a biblioteca `recordlinkage`, podemos implementar essa técnica de forma eficiente e precisa. A Lógica Difusa e algoritmos como o de Levenshtein ajudam a lidar com variações nos dados, melhorando a qualidade das correspondências. No entanto, é importante considerar o custo
