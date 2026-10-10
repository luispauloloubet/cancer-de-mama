# 🎗️ Análise e Modelagem Preditiva de Câncer de Mama

Este repositório contém um projeto completo de Ciência de Dados voltado para a Análise Exploratória de Dados (EDA) e modelagem preditiva utilizando o clássico conjunto de dados de Câncer de Mama (`breast-cancer`). O objetivo principal é estruturar um pipeline analítico de ponta a ponta, aplicando boas práticas de engenharia de software e Machine Learning.

---

## 📌 Sobre o Projeto
O projeto foi desenvolvido com foco em boas práticas de modularização de código (`DRY - Don't Repeat Yourself`), separando lógicas de pré-processamento, configuração, visualização e modelagem em módulos reutilizáveis dentro da pasta `src/`. A solução busca prever diagnósticos e extrair insights valiosos por meio de técnicas estatísticas e algoritmos de aprendizado de máquina.

---

## 📊 Base de Dados
A base de dados utilizada (`breast-cancer.csv`) contém características computadas a partir de imagens digitalizadas de aspirados por agulha fina (PAAF) de massas mamárias. 
* As características descrevem as características dos núcleos celulares presentes na imagem.
* O dataset limpo e otimizado é armazenado em formato **Parquet** (`breast-cancer-clean.parquet`) para garantir maior velocidade de leitura e integridade dos tipos de dados.
* Para mais detalhes, consulte o [Dicionário de Dados](./referencias/01_dicionario_de_dados.md).

---

## 🗂️ Estrutura do Repositório

```text
base_cancer/
│
├── dados/                    # Armazenamento dos dados brutos e tratados
│   ├── breast-cancer.csv     # Base de dados original
│   └── breast-cancer-clean.parquet # Base de dados tratada (Parquet)
│
├── notebooks/                # Jupyter Notebooks organizados por etapas
│   ├── src/                  # Módulos auxiliares em Python
│   │   ├── __init__.py
│   │   ├── auxiliares.py     # Funções utilitárias e de suporte
│   │   ├── config.py         # Configurações globais do projeto
│   │   ├── graficos.py       # Funções padronizadas de visualização
│   │   └── models.py         # Funções de treino e avaliação de modelos
│   ├── 01.EDA.ipynb          # Análise Exploratória de Dados
│   ├── 02.metricas.ipynb     # Avaliação de métricas de desempenho
│   └── 03.modelos.ipynb      # Treinamento e experimentação de modelos
│
├── referencias/              # Documentações de suporte
│   └── 01_dicionario_de_dados.md # Dicionário descritivo das variáveis
│
├── relatorios/               # Relatórios gerados e gráficos salvos
│   └── imagens/
│
├── .env.exemplo              # Exemplo de variáveis de ambiente
├── ambiente.yml              # Configuração de ambiente Conda
├── requirements.txt          # Dependências do projeto (Pip)
├── LICENSE                   # Licença do projeto
└── README.md                 # Documentação principal do repositório
```
---
**Desenvolvido por Luis Paulo Loubet** *Graduando em Engenharia Aeronáutica - EESC-USP*
