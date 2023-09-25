## Curso - Data Science: análise e visualização de dados | Alura

Repositório referente ao curso de introdução a Data Science utilizando bibliotecas do Python para análise e visualização de dados. 

- Arquivos do curso [link](https://github.com/alura-cursos/introducao-a-data-science/archive/aula0.zip)
- Download dos datasets utilizados [link](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata?resource=download)

### Análise Exploratória

No curso foi utilizada a biblioteca **Pandas** para fazer a importação dos datasets, realizar a manipulação e análise dos dados.
Foram abordadas funções para realizar a alteração do nome das variáveis, contagem de valores únicos, cálculo de média e mediana.

```
# Mostra o nome das colunas
notas.columns
# Renomenando as colunas
notas.columns = ['usuarioId', 'filmeId', 'nota', 'momento']
#Mostra as 5 primeiras linhas
notas.head()
```

### Data Visualization

Geração de gráficos com funções plot básicas e com o auxílio das bibliotecas **Matplotlib** e **Seaborn**. Noções básicas de quais visualizações são mais apropriadas para cada tipo de análise e técnicas de manipulação de dados para auxiliar a criação dos gráficos.

```
#Mostra o histograma da coluna Nota
notas['nota'].plot(kind = 'hist')
```

### Estatística