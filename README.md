# 📊 Análise da Evasão Escolar em Escolas Públicas do Distrito Federal

[![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=Streamlit&logoColor=white)](https://streamlit.io)
[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

**Projeto Integrador - Ciência de Dados | Módulo 2**  
**Período de Análise:** 2015-2024 | **Status:** ✅ Concluído

---

## 📌 Sobre o Projeto

Dashboard interativo para análise da evasão escolar nas escolas públicas do Distrito Federal, integrando dados do Censo Escolar (INEP/SEEDF) e políticas públicas como **Pé-de-Meia** e **Escolas Conectadas**.

### Problema Identificado

A evasão escolar representa um desafio crítico nas escolas públicas do DF, especialmente em regiões com maior vulnerabilidade social.

### Hipótese Central

> *"A evasão escolar no DF está relacionada à reprovação, distorção idade-série, vulnerabilidade social e baixa frequência escolar."*

### Estatísticas Iniciais

| Indicador | Valor |
|-----------|-------|
| Estudantes no DF (2024) | 77.000+ (ensino médio) |
| Regiões Administrativas | 31 RAs |
| Período analisado | 10 anos (2015-2024) |
| Registros processados | 71.035+ |

---

## 🏛️ Políticas Públicas Analisadas

### 💰 Programa Pé-de-Meia (Lei nº 14.818/2024)

| Componente | Detalhamento |
|------------|--------------|
| Benefício mensal | R$ 200,00 (frequência ≥ 80%) |
| Bônus anual | R$ 1.000,00 por aprovação |
| Beneficiários no DF | 61.943 estudantes |
| Investimento nacional | R$ 18,6 bilhões |
| Impacto no abandono | Redução de **43%** |

### 🖧 Escolas Conectadas (Decreto nº 11.646/2023)

| Indicador | Situação |
|-----------|----------|
| Conectividade (2026) | 71,7% das escolas |
| Estudantes beneficiados | 24 milhões |
| Investimento total | R$ 3 bilhões |
| Impacto na evasão | **18% menor** |

---

## 📊 Fontes de Dados

| Fonte | Dados | Uso |
|-------|-------|-----|
| **SEEDF** | Situação do aluno, matrículas | Cálculo da evasão |
| **Hugging Face** | Censo Escolar 2015-2024 | Série histórica |
| **IPEDF/Anuário** | Estudos e indicadores | Contextualização |

🔗 **Links:**
- [SEEDF Dados Abertos](https://data.se.df.gov.br/)
- [Censo Escolar HF](https://huggingface.co/datasets/Horusprg/censo-2015-2024)
- [IPEDF](https://www.ipedf.df.gov.br/)

---

## 🔄 Pipeline de Dados (ETL)
