<h1>Machine Learning - Regressão Linear</h1>
<h1> Módulo 25.11 - Ebac</h1>

> **Nota:**
> A apresentação do Readme.md referente a este projeto ainda esta em fase de desenvolvimento, em breve terá novas atualizações...

![Static Badge](https://img.shields.io/badge/-Seaborn-3776AB?style=flat&logo=python&logoColor=white&size=40x40) ![Static Badge](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white) ![Static Badge](https://img.shields.io/badge/-pandas-05122A?style=flat&logo=pandas) ![Static Badge](https://img.shields.io/badge/-Numpy-013243?&logo=NumPy) ![Static Badge](https://img.shields.io/badge/-Matplotlib-000000?style=flat&logo=python)

![Marketing](https://github.com/Sandro-Alexandre-Olmedo/machine-learning-para-estimativa-do-valor-em-estoque-modulo-25.11-Ebac/blob/b6e5391c09a06242dbf82a4a52ee8e3b549aa498/marketing2.jpg)

# **Introdução**

Grandes empresas têm o seu sucesso alcançado através do marketing, certo? Sim, isso já é bem estabelecido nos atuais mercados em nível global, na verdade as vendas e os estoques estão intimamente relacionadas com o marketing e este último sempre requer atualizações nas estratégias e no planejamento das campanhas de marketing.

Um dos grandes problemas dentro de muitas empresas é com a gestão de estoques, sendo assim, os gestores precisam ser muito eficientes em descobrir exatamente as formas mais adequadas de utilizar os recursos disponíveis para alocar os esforços em marketing e vendas, a fim de que não faltem produtos para atender as demandas dos clientes após as ações de marketing ou que muitos produtos fiquem estagnados nos estoques da empresa após um erro nos valores investidos em campanhas de marketing.

Os gestores precisam saber exatamente o montante físico e em valores que constam no inventário, uso de softwares adequados ajudam muito esse saber e qual deve ser o montante a ser adquirido para outros períodos de acordo com um histórico ou linha de tendência.

O departamento de marketing cria expectativas e promessas a respeito dos produtos através de suas campanhas, no entanto, os profissionais de marketing não têm como estimar exatamente se as mensagens que transmitem ao público são suficientes ou não e para que isso funcione de fato é necessária uma estreita comunicação a com a gestão de vendas e de estoque e garantir que as campanhas de marketing tenham sucesso.

Basicamente uma das formas de estimar corretamente a alocação dos recursos é traçar uma linha de tendência entre os investimentos anteriores em marketing com os montantes em estoque para cada investimento anterior e conhecer melhor a relação entre essas duas variáveis, isso pode ser feito com o auxílio da tecnologia, mais precisamente com o uso do Machine Learning e Regressão Linear e por fim estimar o montante a ser alocado aos estoques após a definição de um determinado valor a ser investido em novas campanhas.
</div>

<div style="text-align: justify; width: 80%; background-color:; border: 0px solid green; line-height: 1.8; font-size: 18px;">

<hr>

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

7 - Grafico de gráfico de dispersão`scatter` com a utilização de um array numpy para traçar uma reta com os valores encontrados através das duas funções `reg_linear.coef_` e `reg_linear.intercept_`; 

8 - Uso da função `reg_linear.predict([[75]])` com o valor a ser investido para prever o montante que deverá ser alocado ao estoque;

9 - Por fim, criação de um novo gráfico de dispersão(scatter) traçando uma reta e marcando um ponto preto no gráfico através do valores ou coordenadas encontrados nas funções `reg_linear.coef_` e `reg_linear.intercept_`;

10 - Resposta;

11 - Storytelling


