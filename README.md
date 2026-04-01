# 🏥 Análise Georreferenciada de Saúde - Niterói/RJ
> **Projeto de Extensão: Tópicos de Big Data em Python**

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Folium](https://img.shields.io/badge/Folium-77B829?style=for-the-badge&logo=Leaflet&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

## 👥 Integrantes
* **Hudson Mata Neves** (Matrícula: 202402852175) - *Engenharia de Dados & ETL*
* **Mauro Henrique Collin Ferreira** (Matrícula: 202403689601) - *Análise Estatística & Geoprocessamento*

## 🎯 Objetivo do Projeto
O objetivo deste projeto é identificar e analisar os **Desertos Assistenciais** de saúde nos bairros de Niterói-RJ. Através do cruzamento de bases demográficas e de infraestrutura, buscamos responder: *A oferta de saúde acompanha o crescimento populacional da cidade?*

## 🛠️ Arquitetura de Dados (Pipeline)
O projeto foi estruturado para ser totalmente portátil e executável via nuvem:
1. **Data Sourcing:** Extração automatizada de CSVs via GitHub e integração de dados hospitalares via API `PySUS` (DataSUS).
2. **Data Cleaning:** Normalização de malhas censitárias e mineração de texto para classificação de gestão (Pública vs Privada).
3. **Analytics:** Cálculo de pressão assistencial, detecção de *Outliers* (Z-Score) e regressão linear de demanda.
4. **Geospatial Visualization:** Geração de mapas coropléticos interativos integrando a malha oficial do IPEA (`geobr`).

## 📊 Fontes e Validação
A veracidade dos dados é o pilar deste projeto. Utilizamos fontes oficiais cruzadas:
- **Demografia:** Censo IBGE 2022.
- **Capacidade:** CNES (Cadastro Nacional de Estabelecimentos de Saúde) via `PySUS`.
- **Validação de Rede:** [FeSaúde Niterói](https://www.fesaude.niteroi.rj.gov.br/nossas-unidades-lista-completa).
- **Contextualização:** Dados de cobertura suplementar da [ANS](https://www.ans.gov.br/).

## 💡 Principais Insights
- **O Fator ANS:** Descobrimos que a alta taxa de planos de saúde em Niterói (aprox. 60%) explica a baixa densidade de unidades públicas em bairros como Icaraí.
- **Unidades de Fronteira:** O Big Data revelou que algumas unidades (ex: MMF Colônia) atendem populações de bairros vizinhos, o que exige uma análise geográfica além do polígono do mapa.
- **Regressão:** A baixa correlação (R²) entre população e número de hospitais sugere uma distribuição histórica centralizada, indicando a necessidade de expansão para a Região Oceânica.

## 🚀 Como Executar
1. Acesse o notebook no [Google Colab](LINK_DO_SEU_COLAB_AQUI).
2. Execute os blocos de importação (os dados serão baixados automaticamente deste repositório).
3. Explore os mapas interativos gerados ao final do código.

---
**Estácio Niterói | 2026.1**# 🏥 Análise de Indicadores de Saúde - Niterói/RJ

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
