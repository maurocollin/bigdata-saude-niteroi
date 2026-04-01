# 🏥 Análise de Indicadores de Saúde - Niterói/RJ

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![Google Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)

Este projeto é uma **Atividade Extensionista** desenvolvida para a disciplina de **Tópicos de Big Data em Python**. O objetivo é analisar a relação entre a densidade populacional e a oferta de infraestrutura de saúde nos bairros de Niterói, Rio de Janeiro.

## 📋 Integrantes do Grupo
* **Hudson Mata neves** - Matrícula: 202402852175
* **Mauro Henrique Collin Ferreira** - Matrícula: 202403689601

## 🚀 Funcionalidades do Projeto
- **Pipeline de Dados:** Integração de bases do IBGE (Censo 2022) e Prefeitura de Niterói.
- **Engenharia de Dados:** Limpeza, normalização e categorização automatizada (Público vs Privado).
- **Análise Estatística:** Detecção de Outliers (Z-Score e IQR), Regressão Linear e Estatística Descritiva.
- **Geoprocessamento:** Criação de Mapas Coropléticos interativos via biblioteca `Folium` e `geobr`.
- **Análise de Capacidade:** Extração de dados de leitos hospitalares via API do `PySUS`.

## 📁 Estrutura de Arquivos
- `Agregados_por_bairros_basico_BR.csv`: Dados populacionais do IBGE.
- `Hospitais.csv`: Unidades hospitalares georreferenciadas.
- `Policlinicas.csv`: Unidades de média complexidade.
- `Unidades_Basicas_de_Saude_UBS.csv`: Unidades de atenção básica.
- `CNES_Leitos_Niteroi.csv`: Dados de capacidade (Leitos SUS e Não-SUS).

## 📊 Principais Insights
O projeto demonstrou matematicamente a existência de "desertos de saúde" em bairros populosos e a falta de correlação direta (R² baixo) entre o crescimento populacional e a oferta de unidades, sugerindo a necessidade de expansão da rede em áreas periféricas.

---
Estácio Niterói - 2026.1
