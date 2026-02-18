# 📊 Análise de Crimes em Chicago (Chicago Crime Analysis)

## 📌 Visão geral

Este projeto realiza uma Análise Exploratória de Dados (EDA) utilizando a base pública de crimes da cidade de Chicago.  
O objetivo é identificar padrões, tendências e insights estratégicos sobre a distribuição de crimes ao longo do tempo e por localização.

A análise foi feita em **Python no Google Colab**, com os dados extraídos diretamente do **Google BigQuery Public Datasets**.

---

## 🎯 Objetivo

Os principais objetivos do projeto são:

- Analisar o volume geral de crimes
- Identificar os tipos de crime mais frequentes
- Encontrar os locais com maior incidência
- Calcular a taxa de prisão (arrest rate)
- Medir a proporção de crimes domésticos
- Entender o comportamento temporal (ano, mês, dia, hora)

Este projeto simula um fluxo real de trabalho de um Analista de Dados: extração → limpeza → análise → visualização → entrega.

---

## 🗂 Fonte de dados

Dataset utilizado:

`bigquery-public-data.chicago_crime.crime`

Fonte: Google Cloud Public Datasets (BigQuery)

A base contém registros detalhados de crimes reportados em Chicago, incluindo:

- Data e hora
- Tipo do crime
- Descrição do local
- Indicador de prisão (arrest)
- Indicador de violência doméstica (domestic)
- Coordenadas geográficas (latitude/longitude)

---

## 🛠 Tecnologias utilizadas

- Python 3
- Pandas
- Pandas-GBQ
- Google BigQuery
- Matplotlib
- Seaborn
- Google Colab
- Looker Studio (Dashboard)

---

## 🔄 Fluxo do projeto

### 1) Extração dos dados
- Conexão com BigQuery usando `pandas-gbq`
- Execução de consulta SQL
- Importação para um DataFrame do Pandas

### 2) Limpeza e preparação
- Conversão da coluna `date` para datetime
- Criação de colunas derivadas de tempo:
  - year
  - month
  - day
  - hour
  - day_of_week
- Tratamento de valores nulos (ward, community_area, latitude, longitude)

### 3) EDA (Análise exploratória)
Principais métricas calculadas:

- Total de casos
- Média diária de crimes
- Crimes por ano
- Crimes por mês
- Top 10 tipos de crime
- Top 10 locais
- Taxa de prisão (%)
- Percentual doméstico (%)

### 4) Visualizações e dashboard
- Gráficos de tendência temporal
- Distribuição por tipo de crime
- Rankings de locais
- KPIs no topo do dashboard
- Dashboard no Looker Studio

---

## 📈 Principais métricas

- 📌 Volume total de crimes
- 📌 Média diária de ocorrências
- 📌 Taxa de prisão (arrest rate)
- 📌 % de crimes domésticos
- 📌 Top categorias de crime
- 📌 Locais com maior incidência

---

## 🔍 Principais insights

(Substitua pelos seus achados reais)

Exemplos:
- Theft e Battery concentram grande parte dos registros.
- Alguns locais têm volume desproporcional de ocorrências.
- A taxa de prisão varia bastante por tipo de crime.
- Existe sazonalidade (picos em determinados meses/períodos).

---

