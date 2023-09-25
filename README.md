### Curso Alura | Data Science: análise e visualização de dados

O curso discorre sobre as técnicas mais básicas e introdutórias da ciência de dados, iniciando o aprendizado pela imputação de dados, análise exploratória, visualização das informações e conceitos de estatística.

- **Arquivos do curso** [link](https://github.com/alura-cursos/introducao-a-data-science/archive/aula0.zip)
- **Download dos datasets** [link](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata?resource=download)

#### Análise Explratória
Utilização da biblioteca **Pandas** para importação e manipulação dos dados, funções para trabalhar com variáveis dos dataframes.

```
# Mostra o nome das colunas
notas.columns
# Renomenando as colunas
notas.columns = ['usuarioId', 'filmeId', 'nota', 'momento']
#Mostra as 5 primeiras linhas
notas.head()
```

### Data Visualization
Trabalhar gerando visualizações básicas usando bibliotecas como **Matplotlib** e **Seaborn**

![Histograma](https://github.com/willyferreira/curso_introducao_data_science/blob/6d36a5b7d18e89a974ca80da53a5f671e2a11dd4/images/hist1.png)