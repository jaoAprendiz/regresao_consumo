# 📘 Regressão Linear - Previsão de Consumo de Água

## 📌 Descrição do Projeto

Este projeto tem como objetivo **prever o consumo de água em unidades residenciais** a partir de variáveis como preço da água, tempo (mês e ano) e blocos do prédio. O modelo utiliza **Regressão Linear Múltipla** para identificar fatores que influenciam o consumo e auxiliar na gestão mais eficiente dos recursos.

O trabalho foi desenvolvido em **Python**, dentro de um **Jupyter Notebook**, e segue um fluxo estruturado de análise de dados: exploração, limpeza, modelagem e avaliação.

---

## 🎯 Objetivos

1. Prever o consumo de água de cada unidade.
2. Tratar dados nulos e valores inválidos (como consumos negativos).
3. Construir dois modelos de regressão linear múltipla:

   * **Modelo 1:** utilizando todas as variáveis.
   * **Modelo 2:** utilizando apenas variáveis estatisticamente significativas (p-valor < 0.05).
4. Avaliar o desempenho de cada modelo e interpretar os resultados.

---

## 📂 Estrutura do Projeto

* **📘 Introdução** → Contexto e objetivos.
* **📂 Importação das Bibliotecas** → Bibliotecas utilizadas.
* **📊 Exploração dos Dados** → Análise inicial, tratamento de nulos e inconsistências.
* **🔍 Análise Exploratória** → Gráficos, distribuições e correlações.
* **⚙️ Preparação dos Dados** → Seleção de variáveis, criação da variável `consumption`.
* **🧠 Modelagem (Regressão Linear)** → Construção dos dois modelos.
* **📈 Avaliação** → Comparação de métricas (R², RMSE) e interpretação estatística.
* **🚀 Conclusão** → Insights e próximos passos.

---

## 🛠️ Tecnologias Utilizadas

* [Python 3](https://www.python.org/)
* [Pandas](https://pandas.pydata.org/)
* [NumPy](https://numpy.org/)
* [Matplotlib](https://matplotlib.org/)
* [Seaborn](https://seaborn.pydata.org/)
* [Scikit-learn](https://scikit-learn.org/)
* [Statsmodels](https://www.statsmodels.org/)
* [Jupyter Notebook](https://jupyter.org/)

---

## 📊 Resultados e Insights

### 🔹 Primeiro Modelo

* Considerou todas as variáveis (preço, mês, ano e blocos).
* Apresentou **baixo poder explicativo (R² ≈ 0.097)**.
* Mostrou que **preço, mês, ano e Bloco A** influenciam o consumo, mas outros fatores também são determinantes.

### 🔹 Segundo Modelo

* Incluiu todos os blocos explicitamente.
* Obteve **R² ≈ 0.798**, explicando quase **80% da variação no consumo**.
* Revelou que:

  * **Preço maior → consumo menor**.
  * **Mês/ano → evidenciam sazonalidade e tendência de crescimento**.
  * **Blocos → ajudam a explicar diferenças de consumo entre unidades**.
* Contudo, apresentou problemas de **multicolinearidade** e alguns blocos não foram estatisticamente significativos.

---

## 🚀 Conclusão

O projeto mostrou que é possível prever o consumo de água com boa precisão ao considerar variáveis como preço, tempo e blocos do prédio. O segundo modelo apresentou desempenho muito superior, mas precisa de refinamentos para eliminar variáveis redundantes e resolver problemas de multicolinearidade.

👉 Próximos passos:

* Testar modelos de **regularização (Ridge, Lasso)**.
* Realizar **seleção de variáveis** para eliminar blocos irrelevantes.
* Incluir variáveis externas (clima, número de moradores).
* Explorar modelos de **séries temporais** para captar melhor a sazonalidade.

---

## 📂 Estrutura de Arquivos

```
📦 regressao_consumo_agua
 ┣ 📜 regressao_consumo.ipynb   # Notebook principal do projeto
 ┣ 📜 water_consumption.csv     # Dataset utilizado
 ┗ 📜 README.md                 # Documentação do projeto
```

---

## 📌 Como Executar o Projeto

1. Clone este repositório:

   ```bash
   git clone https://github.com/jaoAprendiz/regressao_consumo_agua.git
   ```
2. Acesse a pasta do projeto:

   ```bash
   cd regressao_consumo_agua
   ```
3. Crie e ative um ambiente virtual (opcional, mas recomendado).
4. Instale as dependências:

   ```bash
   pip install -r requirements.txt
   ```
5. Abra o Jupyter Notebook:

   ```bash
   jupyter notebook regressao_consumo.ipynb
   ```

---

## ✨ Autor

Projeto desenvolvido por **\[João Victor Soave]** 👨‍💻 como estudo de **Regressão Linear aplicada ao consumo de água**.

---

👉 Quer que eu já gere também um **requirements.txt** com base nas bibliotecas usadas no notebook?
