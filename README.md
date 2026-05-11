# 🎓 Faculdade Estácio de Sá
## **Curso:** Análise e Desenvolvimento de Sistemas
### **Disciplina:** Tópicos de Big Data em Python

---

# 📊 **PROJETO EXTENSIONISTA**
## **Tema:** Análise de Indicadores de Saúde Municipal Pública e Privada
### *Previsão de Demandas por Bairro em Niterói-RJ*

---

### **Corpo Docente:**
* **Profª Simone Gama**

### **Corpo Discente (Grupo):**
| Nome | Matrícula |
| :--- | :--- |
| **Hudson Mata Neves** | 202402852175 |
| **Mauro Henrique Collin Ferreira** | 202403689601 |

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

## 📂 Bases de Dados
Os dados são consumidos diretamente deste repositório para garantir a **reprodutibilidade** do estudo:
* `Agregados_por_bairros_basico_BR.csv`: Dados demográficos (IBGE).
* `Unidades_Basicas_de_Saude_UBS.csv`: Infraestrutura de atenção básica.
* `Hospitais.csv` / `Policlinicas.csv`: Rede de média e alta complexidade.
* `CNES_Leitos_Niteroi.csv`: Capacidade hospitalar (Leitos).

## 📊 Como Visualizar
1. Abra o arquivo `TRAB_PRONTO.ipynb`.
2. Utilize o botão **"Open in Colab"** (se disponível) ou execute localmente em um ambiente Jupyter.
3. Certifique-se de ter uma conexão ativa com a internet para que o código possa baixar as bases de dados e a malha geográfica.

---
> **Impacto Social:** Este estudo fornece subsídios técnicos para o planejamento de políticas públicas em Niterói, evidenciando áreas que necessitam de expansão da rede assistencial.
