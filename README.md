# Desafio COMPET - Inteligência Artificial na Prática

## ✅ Objetivo
Desenvolver um sistema de predição utilizando técnicas de Aprendizado de Máquina para resolver um problema de **classificação**.

---

## 🎯 Justificativa da Base de Dados

Escolhi o **Bank Marketing Dataset** por ser uma base do Kaggle amplamente utilizada em estudos de classificação, além de apresentar características importantes para um projeto prático de Inteligência Artificial:

- **Formato adequado**: dados tabulares, compatíveis com o uso de algoritmos clássicos de classificação.
- **Variáveis diversas**: mistura de variáveis categóricas e numéricas, ideal para demonstrar técnicas de pré-processamento.
- **Problema real**: predição da adesão a um produto financeiro, o que possui aplicação prática direta no setor bancário.
- **Dimensão moderada**: número de atributos e instâncias apropriado para análises em ambiente acadêmico, sem exigir recursos computacionais excessivos.

Essa base permite explorar todo o ciclo de desenvolvimento de um modelo de aprendizado supervisionado, desde a análise exploratória até a implementação de uma interface para predição.

---

## 📂 Base de Dados

- **Fonte**: Dataset Kaggle "Bank Marketing Dataset"
- **Link**: [www.kaggle.com/datasets/janiobachmann/bank-marketing-dataset/versions/1?resource=download)
- **Descrição**: Base contendo informações de clientes de um banco, utilizada para prever se o cliente irá aderir a um produto financeiro.

---

## 🛠️ Etapas Realizadas

### 1. Análise Exploratória
- Utilização das bibliotecas `pandas`, `matplotlib` e `seaborn` para:
  - Estatísticas descritivas.
  - Visualizações: gráficos de barras e scatterplots.

### 2. Pré-processamento
- Remoção de variáveis irrelevantes.
- Tratamento de valores faltantes.
- Codificação de variáveis categóricas com `LabelEncoder` e `OneHotEncoder`.

### 3. Modelagem
- Separação da base em treino (70%) e teste (30%).
- Treinamento de dois modelos:
  - **Árvore de Decisão** (`DecisionTreeClassifier`)
  - **Random Forest** (`RandomForestClassifier`)

### 4. Avaliação
- Cálculo da acurácia para ambos os modelos.
- Escolha do modelo com melhor desempenho.

---

## 🏆 Nível II - Avaliação Melhorada

- Realização de **30 execuções** com treino/teste para cada modelo.
- Cálculo da **média** e **desvio padrão** da acurácia.
- Conclusão sobre qual modelo foi:
  - Mais **estável**.
  - Deu o maior **acerto**.

- O melhor modelo foi **salvo** utilizando `pickle`.

### 5. Interface Gráfica
- Criada com a biblioteca `gradio` para entrada de dados e exibição da predição.

---

## 💻 Como Executar

1. Clone este repositório.
2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
