### Curso Alura | Data Science: análise e visualização de dados

O curso discorre sobre as técnicas mais básicas e introdutórias da ciência de dados utilizando a linguagem **Python**, iniciando o aprendizado pela imputação de dados, análise exploratória, visualização das informações e conceitos de estatística.

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

#### Data Visualization
Trabalhar gerando visualizações básicas usando bibliotecas como **Matplotlib** e **Seaborn**

```
#Mostra o histograma da coluna Nota
notas['nota'].plot(kind = 'hist')
```
![Histograma](https://github.com/willyferreira/curso_introducao_data_science/blob/6d36a5b7d18e89a974ca80da53a5f671e2a11dd4/images/hist1.png)

```
#Mostrando boxplot com a média geral dos filmes
sns.boxplot(x = medias_por_filme)
```
![Boxplot com a média de notas dos filmes](https://github.com/willyferreira/curso_introducao_data_science/blob/abd4e0006fd804a4bed8af6fdaf14dbcf70e333e/images/boxplot_medias_por_filme.png)

```
sns.distplot(medias_por_filme)
```
![Distplot](https://github.com/willyferreira/curso_introducao_data_science/blob/abd4e0006fd804a4bed8af6fdaf14dbcf70e333e/images/distplot_medias_por_filme.png)

```
#Mostra o histograma da média dos filmes
plt.hist(medias_por_filme)
plt.title('Histograma das médias dos filmes')
```
![Histograma da média dos filmes](https://github.com/willyferreira/curso_introducao_data_science/blob/abd4e0006fd804a4bed8af6fdaf14dbcf70e333e/images/histograma_medias_dos_filmes.png)

```
#criando gráfico com o dataframe
sns.barplot(x='lingua', y='total', data= dados)
```
![Barplot com informação sobre idioma dos filmes](https://github.com/willyferreira/curso_introducao_data_science/blob/b0cd5e82568a0ff62d2cd3edf6c1015fc97bd7d6/images/barplot_linguagem.png)

```
#catplot
sns.catplot(
    x = 'original_language', kind = 'count', data = filmes_sem_lingua_original_em_ingles,
    aspect = 2,
    palette = 'GnBu_d',
    order = total_por_lingua_de_outros_filmes.index)
```
![Catplot com informação sobre idioma dos filmes](https://github.com/willyferreira/curso_introducao_data_science/blob/b0cd5e82568a0ff62d2cd3edf6c1015fc97bd7d6/images/barplot_linguagem_original.png)

#### Conceitos estatísticos
Conceitos sobre média, mediana, desvio padrão, tendência central e dispersão, e como observar por meio de gráficos como boxplot e histograma.

```
sns.boxplot(x = "filmeId", y = "nota", data = notas.query("filmeId in [1,2,3,4,5]"))
```
![Boxplot Filmes ID 1 a 5](https://github.com/willyferreira/curso_introducao_data_science/blob/b0cd5e82568a0ff62d2cd3edf6c1015fc97bd7d6/images/boxplot_5filmes.png)