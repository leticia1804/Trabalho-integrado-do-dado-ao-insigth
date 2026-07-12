# Trabalho-integrado-do-dado-ao-insigth
# 🌦️ Projeto Integrado – Do Dado ao Insight
Pós-graduação em Ciência de Dados

Projeto Integrado – Do Dado ao Insight

Julho/2025

**Letícia dos Santos**

---

## Monitoramento Climático com Python e Power BI

Este repositório contém o código desenvolvido em **Python** para o Projeto Integrado da Pós-graduação em Ciência de Dados, cujo objetivo foi construir um pipeline simplificado de dados, desde a coleta até a geração de insights por meio de um dashboard no Power BI.

O projeto utiliza dados públicos do **Instituto Nacional de Meteorologia (INMET)** para comparar o comportamento climático entre as estações meteorológicas **Forte de Copacabana** e **Vila Militar**, localizadas na cidade do Rio de Janeiro.

---

# 🎯 Objetivo

Desenvolver um pipeline de Ciência de Dados capaz de:

- Coletar dados meteorológicos públicos do INMET;
- Realizar limpeza, padronização e transformação dos dados utilizando Python;
- Construir uma base consolidada para análise;
- Gerar indicadores para comparação entre as duas estações;
- Exportar uma base tratada para utilização no Power BI;
- Produzir insights que auxiliem na interpretação do comportamento climático.

---

# 🛠 Tecnologias Utilizadas

- Python 3
- Google Colab
- Pandas
- NumPy
- Microsoft Power BI
- Microsoft Azure (conceitual)
- GitHub

---

# 📂 Estrutura do Projeto

```text
Projeto_INMET
│
├── Dados_Brutos
│     ├── dados_A652_H_2025.csv
│     └── dados_A621_H_2025.csv
│
├── Notebook
│     └── Tratamento_INMET.ipynb
│
├── Dados_Tratados
│     └── Base_Final_INMET.csv
│
└── Dashboard
      └── Dashboard.pbix
```

---

# 📊 Etapas Desenvolvidas no Código

O notebook realiza todas as etapas de preparação dos dados.

## 1. Importação dos dados

- Leitura dos arquivos CSV disponibilizados pelo INMET;
- Separação dos metadados das informações meteorológicas.

---

## 2. Limpeza dos dados

Foram realizadas as seguintes etapas:

- Remoção de linhas desnecessárias;
- Ajuste dos nomes das colunas;
- Conversão dos tipos de dados;
- Padronização dos formatos;
- Tratamento de valores ausentes.

---

## 3. Transformações

Durante o processamento foram criadas novas variáveis para facilitar as análises:

- DataHora
- Ano
- Mês
- Nome do mês
- Dia
- Hora
- Estação do ano
- Amplitude térmica

Também foi realizada a união das duas estações em uma única base de dados.

---

## 4. Análise Exploratória

Foram calculadas estatísticas descritivas para compreender o comportamento das variáveis meteorológicas:

- Temperatura média
- Temperatura máxima
- Temperatura mínima
- Umidade relativa
- Precipitação
- Velocidade do vento
- Amplitude térmica

Também foram avaliadas distribuições dos dados e possíveis valores inconsistentes.

---

## 5. Exportação

Ao final do processamento, a base tratada foi exportada para:

```text
Base_Final_INMET.csv
```

Esse arquivo foi utilizado posteriormente na construção do dashboard no Microsoft Power BI.

