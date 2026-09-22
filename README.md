# 🎌 Anime Recommendation System | NLP & Content-Based Filtering

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-F7931E.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

## 📌 Visão Geral do Projeto

Este projeto consiste em um **Sistema de Recomendação de Animes** baseado em filtragem por conteúdo (*Content-Based Filtering*). O objetivo principal é analisar o catálogo de animes, processar suas características textuais utilizando técnicas de **Processamento de Linguagem Natural (NLP)** e recomendar títulos com alta similaridade matemática ao anime consultado pelo usuário.

---

## 🛠️ Tecnologias e Conceitos Aplicados

- **Linguagem:** Python
- **Manipulação de Dados:** Pandas, NumPy
- **Processamento de Linguagem Natural (NLP):** `TfidfVectorizer` (TF-IDF)
- **Métricas de Similaridade:** Similaridade de Cosseno (*Cosine Similarity*)
- **Versionamento:** Git e GitHub

---

## 📐 Como Funciona o Algoritmo?

1. **Tratamento de Dados:** Higienização da base de dados, normalização de caracteres e tratamento de valores nulos nas categorias.
2. **Vetorização (TF-IDF):** Conversão dos gêneros e tags do anime em matrizes numéricas ponderadas, destacando palavras com alto poder descritivo.
3. **Matriz de Similaridade:** Cálculo do ângulo entre os vetores de cada anime na matriz de similaridade de cosseno.
4. **Mecanismo de Recomendação:** A função recupera os $N$ animes com os maiores pontuações de similaridade em relação ao título inserido.

---

## 📁 Estrutura do Repositório

```text
├── data/              # Diretório para armazenamento dos dados
├── notebooks/         # Notebooks Jupyter para análise exploratória e testes
├── src/               # Scripts com módulos reutilizáveis
├── .gitignore         # Arquivos ignorados pelo Git
├── README.md          # Documentação do projeto
└── requirements.txt   # Dependências do projeto
```

---

## 🚀 Como Executar o Projeto

### Pré-requisitos
* Python 3.8 ou superior instalado.
* Dataset `anime.csv` baixado do [Kaggle - Anime Recommendation Database](https://www.kaggle.com/datasets/CooperUnion/anime-recommendations-database).

### Passo a Passo
1. **Clonar o repositório:**
```bash
git clone [https://github.com/evertonvcfranca/anime-recommendation-system.git](https://github.com/evertonvcfranca/anime-recommendation-system.git)
cd anime-recommendation-system
```
2. **Instalar as dependências:**
```bash
pip install -r requirements.txt
```
3. **Adicionar os dados:**
   - Faça o download do arquivo `anime.csv` e insira no diretório `data/raw/`.
4. **Executar o Notebook:**
   - Abra o arquivo `notebooks/01_eda_e_recomendador.ipynb` em seu Jupyter Notebook ou Google Colab.

---

## 👤 Autor
Desenvolvido por **Everton França**
*Estudante de Ciência de Dados | Univesp*
