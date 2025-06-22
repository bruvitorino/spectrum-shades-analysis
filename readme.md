# Exame Prático – Spectrum Shades LLC

Este repositório contém a solução do exame prático proposto pela [DataCamp](https://www.datacamp.com/) para análise de dados da empresa fictícia **Spectrum Shades LLC**, especializada em soluções de coloração para concreto.

---

## Sobre a Empresa

A **Spectrum Shades LLC** fornece pigmentos e sistemas de coloração para aplicações em concreto decorativo, pré-moldado e pavers. Recentemente, a empresa identificou um aumento nas **reclamações de inconsistência na cor dos produtos**, impactando a satisfação dos clientes e gerando potenciais devoluções.

---

## 🎯 Objetivo da Análise

Você faz parte da equipe de dados encarregada de identificar fatores que afetam a **qualidade final dos produtos**, com o objetivo de reduzir variações de cor e melhorar a confiabilidade dos lotes produzidos.

---

## 📁 Arquivo de Dados

- `production_data.csv`: Contém os dados dos lotes de produção, incluindo informações como tipo de fornecedor, tipo e quantidade de pigmento, tempo de mistura, e nota de qualidade do produto final.

---

## ✅ Tarefas Realizadas

### 1. Limpeza de Dados
- Preenchimento de valores ausentes com regras definidas (ex: média, mediana, valores padrão).
- Conversão de colunas para tipos adequados (`datetime`, `str`, etc.).
- Normalização de texto e categorização.

### 2. Análise por Tipo de Fornecedor
- Cálculo da média de:
  - `product_quality_score`
  - `pigment_quantity`
- Agrupamento por `raw_material_supplier`.

### 3. Filtro por Fornecedor Internacional
- Seleção de lotes com `raw_material_supplier = 2` e `pigment_quantity > 35 kg`.
- Cálculo da média de qualidade e quantidade de pigmento nesses casos.

### 4. Estatísticas e Correlação
- Cálculo de média e desvio padrão para:
  - `product_quality_score`
  - `pigment_quantity`
- Cálculo da correlação de Pearson entre pigmento e qualidade.

---

## Ferramentas Utilizadas

- Python 3
- Pandas
- Google Colab / Jupyter Notebook

---

## Como Executar

1. Clone este repositório:

   git clone https://github.com/bruvitorino/spectrum-shades-analysis

2. Abra o notebook no Google Colab ou Jupyter.

3. Carregue o arquivo production_data.csv.

4. Execute célula por célula para acompanhar a análise completa.

📌 Observações

Este projeto foi desenvolvido como parte de um exame prático de análise de dados, com foco em:

- Limpeza de dados reais

- Aplicação de estatísticas básicas

- Preparação de dados para insights de negócio