# 🏥 Análise de Indicadores de Saúde Pública e Privada - Niterói/RJ
> **Atividade Extensionista: Tópicos de Big Data em Python**

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=for-the-badge&logo=plotly&logoColor=white)
![Folium](https://img.shields.io/badge/Folium-77B829?style=for-the-badge&logo=Leaflet&logoColor=white)
![Google Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)

Este projeto realiza uma análise aprofundada da infraestrutura de saúde municipal de Niterói-RJ, utilizando técnicas de Big Data para cruzar dados demográficos do **Censo IBGE 2022** com dados de estabelecimentos de saúde do **CNES (DataSUS)**. O objetivo é identificar desertos assistenciais e avaliar a capacidade hospitalar frente às metas internacionais.

## 👥 Integrantes
* **Hudson Mata Neves** (Matrícula: 202402852175)
* **Mauro Henrique Collin Ferreira** (Matrícula: 202403689601)

## 🎯 Objetivo do Projeto
Através do cruzamento de bases demográficas e de infraestrutura, o projeto busca responder: **A oferta de saúde de Niterói acompanha o crescimento populacional por bairro?** Utilizamos ferramentas estatísticas e geográficas para mapear a pressão assistencial na cidade.

## 🛠️ Arquitetura de Dados (Pipeline)
O projeto foi estruturado para ser totalmente portátil e executável em nuvem:
1. **Extração (ETL):** Carga automatizada de CSVs via GitHub e integração de dados de leitos via API `PySUS`.
2. **Qualidade e Veracidade:** Normalização de strings (caracteres especiais e acentos) e mineração de texto para classificação automática de gestão (**Pública vs Privada**).
3. **Analytics & Big Data:** * Detecção de *Outliers* de demanda através de **Z-Score** e **IQR**.
    * **Regressão Linear** para correlacionar população vs. número de unidades.
    * Cálculo de resíduos para identificar anomalias no planejamento urbano.
4. **Visualização Espacial:** Mapas interativos com marcadores georreferenciados e **Mapas Coropléticos** baseados na malha oficial do IPEA (`geobr`).

## 💡 Principais Insights e Funcionalidades
- **O Fator ANS:** A análise sugere que a alta cobertura suplementar em bairros como Icaraí justifica a baixa presença de unidades públicas, enquanto bairros como Fonseca apresentam alta pressão assistencial no SUS.
- **Regressão e Resíduos:** O modelo demonstrou que a oferta de unidades básicas não cresce na mesma proporção que a população (R² baixo), sinalizando a necessidade de expansão da rede.
- **Capacidade OMS:** O projeto avalia o indicador de leitos por 1.000 habitantes, comparando a realidade local com a meta da **Organização Mundial da Saúde (3 a 5 leitos/mil hab)**.
- **O Fator Saúde Suplementar:** O cruzamento de dados revelou que bairros como Icaraí aparecem como 'desertos assistenciais públicos'. No entanto, ao integrar dados da ANS, observamos que cerca de 50% da população de Niterói possui plano de saúde, com concentrações que ultrapassam 80% em bairros nobres, o que altera a interpretação de necessidade de novas UBS nessas áreas específicas.
- **Fonte: ANS** - Agência Nacional de Saúde Suplementar. Caderno de Informações de Saúde Suplementar (Beneficiários por Município).

## 🚀 Como Executar
1. Acesse o notebook através do seu ambiente Python ou [Google Colab](https://colab.research.google.com/).
2. Certifique-se de instalar as dependências necessárias:
   ```bash
   pip install pandas numpy matplotlib seaborn plotly folium scipy scikit-learn geobr pyproj
