<h1>Machine Learning</h1>
<h1>Regressão Linear</h1>
<h1> Módulo 25.11 - Ebac</h1>

> **Nota:**
> A apresentação do Readme.md referente a este projeto ainda esta em fase de desenvolvimento, em breve terá novas atualizações...

![Static Badge](https://img.shields.io/badge/-Seaborn-3776AB?style=flat&logo=python&logoColor=white&size=40x40) ![Static Badge](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white) ![Static Badge](https://img.shields.io/badge/-pandas-05122A?style=flat&logo=pandas) ![Static Badge](https://img.shields.io/badge/-Numpy-013243?&logo=NumPy) ![Static Badge](https://img.shields.io/badge/-Matplotlib-000000?style=flat&logo=python)

![Marketing](https://github.com/Sandro-Alexandre-Olmedo/machine-learning-para-estimativa-do-valor-em-estoque-modulo-25.11-Ebac/blob/b6e5391c09a06242dbf82a4a52ee8e3b549aa498/marketing2.jpg)



<div style="text-align: justify; width: 80%; background-color:; border: 0px solid green; line-height: 1.8; font-size: 18px;">

# **Process Mapping**

**Bibliotecas usadas no projeto:**
- import pandas as pd
- import numpy as np
- import seaborn as sns
- import matplotlib.pyplot as plt
- from sklearn import linear_model
<hr>

1 - Carregamento e leitura de um arquivo CSV com o Pandas;

2 - Exploração dos dados;

3 - Grafico de apresentação `scatter` com `Seaborn`;

4 - Machine Learning e Regressão Linear com o `sklearn`;

5 - Ajustes dos dados do modelo de regressão linear com o método `.fit`, para localizar o coeficiente angular através da função ` reg_linear.coef_`. Esse coeficiente é uma medida que indica a inclinação da reta em relação ao eixo x do plano cartesiano;

6 - Posteriormente o `reg_linear.intercept_` ou intercepto nos trouxe o valor de `y` quando `x` = 0. Em outras palavras, ele indica onde a linha da regressão cruza o eixo `y`, `intercept_` é um atributo do objeto após o modelo ser treinado, ele armazena o valor do intercepto, esse valor será um ponto indicado em um gráfico ligando o eixo `x` com o eixo `y` (correlação);

7 - Grafico de gráfico de dispersão`scatter` com a utilização de um array numpy para traçar uma reta.
Uso dos valores encontrados através das duas funções `reg_linear.coef_` e `reg_linear.intercept_` para traçar uma reta entre os eixos x e y em um gráfico de dispersão(scatter) do pacote Matplotlib, a reta quase que liga boa parte dos pontos, sendo assim, temos uma correlação positiva entre as variáveis, o que nos permite assumir esse modelo de regressão linear é válido na predição ou estimativa do montante em estoque após o investimento sugerido, ou seja, a relação entre valores gastos com marketing e o montante em estoque são boas;

8 - Uso da função `reg_linear.predict([[75]])` com o valor a ser investido para prever o montante que deverá ser alocado ao estoque;

9 - Por fim, criação de um novo gráfico de dispersão(scatter) traçando uma reta e marcando um ponto preto no gráfico através do valores ou coordenadas encontrados nas funções `reg_linear.coef_` e `reg_linear.intercept_`;

10 - Resposta;

11 - Storytelling
Nota: A reta quase que liga boa parte dos pontos, sendo assim, temos uma correlação positiva entre as variáveis, o que nos permite assumir que esse modelo de regressão linear de predição ou estimativa do montante em estoque é boa, ou seja, a relação entre valores gastos com marketing e o montante em estoque estão corretas.
