# Tech Challenge — Fase 1 | Análise Executiva E-commerce Olist

> **POSTECH — Pós-graduação em Data Analytics**
> Análise estratégica de desempenho comercial, eficiência logística e satisfação do cliente baseada no Brazilian E-Commerce Public Dataset by Olist.

[![Status](https://img.shields.io/badge/Status-Concluído-1f4e79?style=flat-square)]()
[![Python](https://img.shields.io/badge/Python-3.10+-1f4e79?style=flat-square&logo=python&logoColor=white)]()
[![Pandas](https://img.shields.io/badge/Pandas-2.x-1f4e79?style=flat-square&logo=pandas&logoColor=white)]()
[![Colab](https://img.shields.io/badge/Google%20Colab-Notebook-1f4e79?style=flat-square&logo=googlecolab&logoColor=white)]()

---

## 📌 Sobre o projeto

Este repositório contém a entrega completa do **Tech Challenge — Fase 1** do curso de pós-graduação em Data Analytics da POSTECH/FIAP. O desafio propõe a construção de um **relatório executivo voltado a investidores e acionistas** do setor de e-commerce, baseado em dados reais de aproximadamente **93 mil pedidos** da Olist no período de **set/2016 a jul/2018**.

O objetivo é **transformar dados transacionais em uma narrativa clara** sobre desempenho comercial, eficiência logística e satisfação do cliente — culminando em recomendações acionáveis para a tomada de decisão estratégica.

---

## 👤 Autoria

| | |
|---|---|
| **Nome** | Ana Paula Corrêa Galdino |
| **Matrícula** | RM370461 |
| **E-mail** | ana.galdiino@outlook.com |
| **Curso** | Pós-graduação em Data Analytics — POSTECH/FIAP |
| **Fase** | 1 |
| **Data** | Abril de 2026 |

---

## 🎯 Indicadores-chave da análise

| Métrica | Valor |
|---|---:|
| Pedidos analisados | **92.909** |
| Receita total | **R$ 15,1 mi** |
| Ticket médio | **R$ 162,03** |
| Tempo médio de entrega | **12,4 dias** |
| Taxa de atraso | **7,7%** |
| Nota média (1 a 5) | **4,07** |
| Estados cobertos | **27** |
| Período coberto | **set/2016 a jul/2018** |

---

## 📂 Estrutura do repositório

```
.
├── README.md                                          ← Este arquivo
├── notebook/
│   └── TECH_CHALLENGE.ipynb                           ← Notebook completo da análise
├── relatorio/
│   └── Tech_Challenge_Relatorio_Executivo_Olist.docx  ← Relatório executivo (8 seções)
├── apresentacao/
│   └── Tech_Challenge_Apresentacao_Executiva_Olist.pptx ← Slides (10 slides, 16:9)
├── roteiro/
│   └── Tech_Challenge_Roteiro_Video_Olist.docx        ← Roteiro cronometrado do vídeo
├── video/
│   └── link_video.txt                                 ← Link do vídeo de até 5 minutos
└── data/
    └── README.md                                      ← Instruções de download do dataset
```

---

## 📊 Conteúdo da análise

A análise está estruturada em cinco grandes blocos, cobrindo as trilhas analíticas sugeridas no enunciado:

### 1. Crescimento e Receita
- Evolução mensal de pedidos, receita e ticket médio
- Pico de Black Friday (nov/2017) e estabilização do patamar operacional
- Top 10 categorias por receita, ticket médio e participação

### 2. Logística e SLA
- Distribuição de tempo de entrega e identificação do ponto de inflexão (20 dias)
- Correlação entre atrasos e nota de satisfação (queda de 39%)
- Mapa de calor: faixa de entrega × ocorrência de atraso
- Categorias com maior peso de frete sobre receita

### 3. Comportamento e Pagamentos
- Distribuição de meios de pagamento (cartão concentra ~78% da receita)
- Comportamento de parcelamento
- Frequência de compra e oportunidade de retenção

### 4. Satisfação do Cliente
- Distribuição de avaliações (77% são 4 ou 5 estrelas)
- Drivers principais de satisfação
- Identificação de risco de churn

### 5. Análise Regional
- Concentração geográfica de receita (SP, RJ, MG = 65%)
- Estados com maior taxa de atraso (Norte e Nordeste em destaque)
- Cruzamento receita × satisfação por estado

---

## 💡 Recomendações estratégicas

A análise resulta em **5 recomendações acionáveis** com problema, solução e impacto esperado:

| # | Recomendação | Impacto esperado |
|:-:|---|---|
| 1 | Reduzir entregas acima de 20 dias | Nota geral de 4,07 → 4,25 |
| 2 | Recalibrar promessa de prazo na vitrine | -30% a -50% nos atrasos percebidos |
| 3 | Programa de retenção e recompra | +R$ 750 mil/ano em receita incremental |
| 4 | Otimização de frete em categorias críticas | -5 a -10 p.p. no peso do frete |
| 5 | Expansão em categorias secundárias | +15% a +25% nas categorias do top 10 |

---

## 🛠️ Stack técnica

- **Linguagem**: Python 3.10+
- **Ambiente**: Google Colab
- **Bibliotecas principais**:
  - `pandas` — manipulação e análise de dados
  - `matplotlib` — visualizações base
  - `seaborn` — heatmaps e gráficos estatísticos
  - `numpy` — operações numéricas

---

## 🎨 Padrão visual

Toda a comunicação visual segue paleta executiva **monocromática azul**, garantindo leitura objetiva e profissional:

| Cor | Hex | Uso |
|---|---|---|
| Azul escuro | `#1f4e79` | Destaques, dados-chave |
| Azul claro | `#a6c8e0` | Base, dados de apoio |
| Cinza claro | `#d9d9d9` | Contexto, dados secundários |
| Branco | `#ffffff` | Fundo |

A escolha por paleta azul sem cores quentes (vermelho, amarelo, verde) mantém o foco na mensagem analítica e evita interpretações emocionais automáticas.

---

## 📥 Como reproduzir a análise

### 1. Clone o repositório
```bash
git clone https://github.com/<seu-usuario>/<nome-do-repo>.git
cd <nome-do-repo>
```

### 2. Baixe o dataset
O dataset não é versionado neste repositório (~50 MB). Faça o download diretamente do Kaggle:

🔗 [Brazilian E-Commerce Public Dataset by Olist — Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

Após baixar, extraia os arquivos CSV na pasta `data/`. Os arquivos esperados são:

```
data/
├── olist_orders_dataset.csv
├── olist_customers_dataset.csv
├── olist_order_items_dataset.csv
├── olist_order_payments_dataset.csv
├── olist_order_reviews_dataset.csv
├── olist_products_dataset.csv
└── olist_sellers_dataset.csv
```

### 3. Execute o notebook
Abra `notebook/TECH_CHALLENGE.ipynb` no Google Colab ou Jupyter e execute as células sequencialmente.

```bash
# Ou via terminal com Jupyter
jupyter notebook notebook/TECH_CHALLENGE.ipynb
```

### 4. Consulte os entregáveis
- **Relatório executivo** em `relatorio/`
- **Slides** em `apresentacao/`
- **Roteiro do vídeo** em `roteiro/`

---

## 📚 Referências

### Dataset
- OLIST. *Brazilian E-Commerce Public Dataset by Olist*. Kaggle, 2018. Disponível em: [kaggle.com/datasets/olistbr/brazilian-ecommerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

### Bibliografia metodológica
- McKinney, W. *pandas: a Foundational Python Library for Data Analysis and Statistics*. PyData, 2011.
- Hunter, J. D. *Matplotlib: A 2D Graphics Environment*. Computing in Science & Engineering, vol. 9, no. 3, 2007.
- Waskom, M. *seaborn: statistical data visualization*. Journal of Open Source Software, 2021.
- Few, S. *Show Me the Numbers: Designing Tables and Graphs to Enlighten*. 2nd ed. Analytics Press, 2012.
- Knaflic, C. N. *Storytelling with Data: A Data Visualization Guide for Business Professionals*. Wiley, 2015.
- Tufte, E. R. *The Visual Display of Quantitative Information*. 2nd ed. Graphics Press, 2001.

### Contexto de mercado
- EBIT/NIELSEN. *Webshoppers* — Relatórios anuais sobre o e-commerce brasileiro.
- ABComm — Associação Brasileira de Comércio Eletrônico. Indicadores de mercado.

---

## 📜 Licença e uso

Este projeto foi desenvolvido como entrega acadêmica do programa POSTECH/FIAP. O dataset é público e pertence à Olist (publicado no Kaggle sob CC BY-NC-SA 4.0). O conteúdo analítico, o relatório, os slides e o código deste repositório são de autoria de **Ana Paula Corrêa Galdino**.

Sinta-se à vontade para usar como referência de estudo, citando a fonte.

---

## 📬 Contato

**Ana Paula Corrêa Galdino**
📧 ana.galdiino@outlook.com
🎓 POSTECH — Pós-graduação em Data Analytics

---

<p align="center">
  <i>Tech Challenge — Fase 1 | Abril 2026</i>
</p>
