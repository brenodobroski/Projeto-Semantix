# ⚡ Análise Preditiva de Consumo de Energia Residencial 💡

![Python](https://img.shields.io/badge/Python-3.11+-blue.svg?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-black?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-006699.svg?style=for-the-badge&logo=xgboost&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811.svg?style=for-the-badge&logo=powerbi&logoColor=black)

## 🎯 Visão Geral do Projeto

Este projeto de ponta a ponta mergulha em mais de 2 milhões de registos de consumo de energia de uma residência para desvendar os padrões ocultos na rotina de uma família. O objetivo final é construir e otimizar um modelo de Machine Learning de alta performance para prever o consumo de energia horário, transformando dados brutos em inteligência acionável.

O trabalho demonstra um fluxo completo de ciência de dados, desde a limpeza e análise exploratória até à engenharia de features, modelagem robusta com validação cruzada para séries temporais e, finalmente, a interpretação dos resultados.

---

## ✨ Destaques do Projeto

* **Análise Exploratória Profunda (EDA):** Identificação de padrões sazonais, semanais e diários que revelam a "história" por trás dos dados.
* **Engenharia de Features:** Criação de variáveis de tempo, lag e janelas móveis para dar ao modelo um contexto temporal rico.
* **Modelagem Robusta:** Comparação entre `RandomForest` e `XGBoost`, com otimização de hiperparâmetros via `GridSearchCV`.
* **Metodologia para Séries Temporais:** Uso correto de `TimeSeriesSplit` para validação cruzada, garantindo uma avaliação honesta e evitando o vazamento de dados.
* **Diagnóstico de Modelo:** Identificação e correção de um problema de *Data Leakage*, demonstrando uma análise crítica dos resultados.
* **Comunicação Visual:** Desenvolvimento de um dashboard interativo no Power BI para apresentar os resultados de forma clara e acessível.

---

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3.11
* **Bibliotecas Principais:**
    * `Pandas` & `NumPy` para manipulação de dados.
    * `Matplotlib` & `Seaborn` para visualização.
    * `Scikit-learn` para modelagem e avaliação.
    * `XGBoost` para o modelo de gradient boosting.
* **Ambiente:** Jupyter Notebook
* **Dashboard:** Microsoft Power BI

---

## 📊 Principais Descobertas (EDA)

A análise exploratória revelou insights fascinantes sobre a rotina da casa:

* **❄️ O Inverno é o Vilão:** O consumo de energia atinge picos nos meses de inverno, impulsionado pelo aquecimento, sendo responsável pela maior parte do gasto anual.
* **🎉 A Casa Vive no Fim de Semana:** O consumo médio no sábado e domingo é significativamente maior do que nos dias úteis.
* **🌙 Picos de Consumo Noturnos:** A rotina diária mostra picos de consumo claros pela manhã e, principalmente, à noite, quando a casa está mais ativa.
* **🔌 Climatização Domina:** O circuito de aquecimento e ar condicionado foi identificado como o maior consumidor de energia entre as áreas monitorizadas.

---

## 🤖 Performance do Modelo

Após a otimização e a correção do data leakage, o modelo campeão **XGBoost** alcançou uma performance excelente no conjunto de teste final, demonstrando sua capacidade de prever o consumo de energia com alta precisão.

| Modelo        | MAE (Erro Médio Absoluto) | R² (Coeficiente de Determinação) |
|---------------|---------------------------|----------------------------------|
| **XGBoost** | **0.1578 kW** | **91.79%** |
| Random Forest | 0.1400 kW                 | 92.20%                           |

Apesar do Random Forest apresentar métricas ligeiramente superiores, o **XGBoost foi escolhido como o modelo final** devido ao seu comportamento de previsão mais estável e confiável, especialmente na captura de picos de consumo.

---

## 🚀 Como Executar o Projeto

1.  **Clone este repositório:**
    ```bash
    git clone [URL_DO_SEU_REPOSITORIO]
    ```
2.  **Crie um ambiente virtual (recomendado):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # No Windows: venv\Scripts\activate
    ```
3.  **Instale as dependências:**
    ```bash
    pip install -r requirements.txt
    ```
    *(**Nota:** Você precisará criar um ficheiro `requirements.txt` com as bibliotecas do seu projeto. Pode fazer isso com o comando `pip freeze > requirements.txt` no seu terminal)*

4.  **Execute o Jupyter Notebook:**
    ```bash
    jupyter notebook "Projeto Semantix - Breno Dobroski.ipynb"
    ```
5. Como a base é grande para o github. baixe ela abaixo
   https://drive.google.com/file/d/1SYIrwp9iz-tiPaeYRCudqR5dzyWXTnVr/view?usp=sharing

---

## 👨‍💻 Autor

* **Breno Dobroski**
* **LinkedIn:** linkedin.com.br/in/brenodobroski
