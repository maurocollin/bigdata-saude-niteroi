# 🎓 Faculdade Estácio de Sá
## **Curso:** Análise e Desenvolvimento de Sistemas
### **Disciplina:** Tópicos de Big Data em Python

---

### 📊 **PROJETO EXTENSIONISTA**
## **Tema:** Análise de Indicadores de Saúde Municipal Pública e Privada
### *Previsão de Demandas por Bairro em Niterói-RJ*

---

### **Corpo Docente:**
* **Profª: Simone Ingrid Monteiro Gama**

### **Corpo Discente (Grupo):**
| Nome | Matrícula | Função no Projeto |
| :--- | :--- | :--- |
| **Hudson Mata Neves** | 202402852175 | Analista de Dados |
| **Mauro Henrique Collin Ferreira** | 202403689601 | Engenheiro de Dados |

---

## 📝 Sobre o Projeto
Este projeto de **Big Data Analytics** visa analisar a infraestrutura de saúde (pública e privada) do município de Niterói-RJ, cruzando dados demográficos do IBGE com dados de capacidade instalada do CNES e prefeituras. O objetivo é identificar "desertos assistenciais" e prever demandas baseadas no crescimento populacional, atendendo aos requisitos de um **Trabalho Extensionista** com impacto social direto.

## 🛠️ Tecnologias Utilizadas
* **Linguagem:** Python 3.x
* **Ambiente:** Google Colab / Jupyter Notebook
* **Principais Bibliotecas:**
  * `Pandas` & `Numpy`: Manipulação e Auditoria de Dados.
  * `Matplotlib` & `Seaborn`: Visualização Estatística.
  * `Plotly`: Gráficos de Regressão Interativos.
  * `Folium` & `Geobr`: Geoprocessamento e Mapas Coropléticos.
  * `Scikit-Learn`: Modelagem Preditiva (Regressão Linear).

## 🚀 Estrutura da Análise (8 Etapas)
O projeto foi desenvolvido seguindo um rigoroso fluxo de engenharia de dados:

1.  **Ingestão e Diagnóstico Estrutural:** Carga automatizada via GitHub e auditoria de tipos (`dtypes`).
2.  **Auditoria de Integridade:** Identificação de nulos e duplicatas (Pré-processamento).
3.  **Consolidação da Tabela Analítica:** Cruzamento (Merge) entre bases de Saúde e População.
4.  **Estatística Descritiva:** Análise quantitativa de oferta e demanda.
5.  **Análise Preditiva:** Modelagem de Regressão Linear com análise de resíduos e $R^2$.
6.  **Análise Diagnóstica Espacial:** Mapeamento geográfico da rede hospitalar.
7.  **Análise Territorial de Cobertura:** Identificação visual de zonas de assistência.
8.  **Análise Prescritiva (OMS):** Validação da capacidade instalada frente aos indicadores da Organização Mundial da Saúde.

## 📂 Fontes de Dados
Os dados foram obtidos de bases governamentais oficiais e são consumidos diretamente deste repositório para garantir a **reprodutibilidade** e a precisão da análise:

* `Agregados_por_bairros_basico_BR.csv`: * **Dados Demográficos (IBGE):** [Censo 2022 - Agregados por Bairros](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/Agregados_por_Bairro_csv/)
    * *Dicionário de dados:* [IBGE Dicionário](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Agregados_por_Setores_Censitarios/)
* `CNES_Leitos_Niteroi.csv`: * **Capacidade Hospitalar (DATASUS/CNES):** [CNES - Base de Dados de Leitos](https://cnes.datasus.gov.br/pages/downloads/arquivosBaseDados.jsp)
    * *Dicionário de dados:* [CNES Dicionário](https://cnes.datasus.gov.br/EstatisticasServlet?path=SCNES_DICIONARIO_DE_DADOS.ZIP)
* **Infraestrutura de Saúde (SIGeo Niterói):**
* `Hospitais.csv`: * [Hospitais de Niterói](https://www.sigeo.niteroi.rj.gov.br/maps/7636a753146a426ba56aa15ef086e178)
* `Policlinicas.csv`:  * [Policlínicas de Niterói](https://www.sigeo.niteroi.rj.gov.br/maps/c7f2ebff746a4b1fb3a69999b8c04598)
* `Unidades_Basicas_de_Saude_UBS.csv`:    * [Unidades Básicas de Saúde (UBS)](https://www.sigeo.niteroi.rj.gov.br/maps/c6c3183b85a24e1bb46a17d89aa55d5f)

## 📊 Como Visualizar
1. Abra o arquivo `TRAB_PRONTO.ipynb`.
2. Utilize o botão **"Open in Colab"** (se disponível) ou execute localmente em um ambiente Jupyter.
3. Certifique-se de ter uma conexão ativa com a internet para que o código possa baixar as bases de dados e a malha geográfica.

## 🤖 Declaração de Uso de Inteligência Artificial (IA)

Em conformidade com as diretrizes da disciplina, declaramos o uso de ferramentas de Inteligência Artificial Generativa (principalmente o **Google Gemini**, com suporte auxiliar do **ChatGPT** em demandas específicas) para auxiliar no desenvolvimento deste projeto. 

As IAs foram utilizadas de forma assistiva, crítica e supervisionada para os seguintes fins:
* **Planejamento e Arquitetura:** Sugestão de fluxo de trabalho (início, meio e fim) e adoção de boas práticas de Engenharia e Ciência de Dados.
* **Engenharia de Dados (Etapa 3):** Auxílio na estruturação dos códigos de agregação, cruzamento de bases (*merge*) e na auditoria final de qualidade da Tabela Analítica.
* **Visualização de Dados (Etapa 5 - Análise Preditiva):** Geração do código específico para ajuste de layout (inclinação dos rótulos dos bairros em 45º) no gráfico, melhorando a legibilidade visual.
* **Code Review:** Revisão e validação pontual do código desenvolvido pela dupla ao longo das etapas, buscando otimização e correção de pequenos erros.

---
> **Impacto Social:** Este estudo fornece subsídios técnicos para o planejamento de políticas públicas em Niterói, evidenciando áreas que necessitam de expansão da rede assistencial.
