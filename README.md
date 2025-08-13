Este relatório apresenta uma análise detalhada dos fatores que mais influenciam a evasão de clientes em uma empresa de telecomunicações. Baseando-se no desempenho de dois modelos de machine learning, Árvore de Decisão e Regressão Logística, este estudo visa identificar os principais motivos de cancelamento e propor estratégias de retenção eficazes e baseadas em dados.

## 📓 Descrição do projeto
### 🗃️ Preparação dos Dados
A preparação dos dados foi um passo crucial para garantir a qualidade da nossa análise e do modelo. As seguintes etapas foram realizadas:

Classificação de Variáveis: As variáveis do nosso conjunto de dados foram classificadas em numéricas e categóricas.

Separação em Treino e Teste: Para avaliar o desempenho do nosso futuro modelo, o conjunto de dados foi dividido em duas partes: 80% para o treino do modelo e 20% para o teste. Isso garante que o modelo seja avaliado em dados que ele nunca viu antes, evitando o problema de overfitting.

### 📈 Análise Exploratória dos Dados (EDA)
A Análise Exploratória dos Dados nos permitiu extrair insights valiosos antes de construir o modelo. A investigação focou na relação entre cancelamentos e variáveis importantes, utilizando gráficos para a visualização.

Tempo de Contrato e Evasão: Através de um boxplot, foi possível observar que clientes que evadiram tendem a ter um tempo de contrato menor do que aqueles que permanecem na empresa.

Total Gasto e Evasão: A análise em boxplot mostrou que clientes que cancelam geralmente têm um gasto total mais baixo.

Relação Múltipla: Um gráfico de scatter plot mostrou que a maioria dos clientes que cancelam são aqueles que possuem pouco tempo de contrato e pouco total gasto, reforçando as conclusões anteriores.

## Como Executar o Notebook

Para executar este notebook, você precisará ter as seguintes bibliotecas Python instaladas:

```bash
  import pandas as pd
  import seaborn as sns
  import matplotlib.pyplot as plt
  from sklearn.preprocessing import StandardScaler
  from sklearn.compose import make_column_transformer, make_column_selector
  from sklearn.preprocessing import OneHotEncoder
```
Após instalar as bibliotecas, o notebook pode ser executado em qualquer ambiente que suporte arquivos .ipynb. Certifique-se de que o arquivo CSV (df_limpo) esteja no mesmo diretório do notebook para que os dados possam ser carregados corretamente.
