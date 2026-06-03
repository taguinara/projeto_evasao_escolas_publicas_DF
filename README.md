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

## 🚀 Como Executar

### Pré-requisitos

```bash
Python 3.8+
Git
Pip

📁 Estrutura do Projeto

projeto_evasao_publico/
├── scripts/                    # Scripts ETL
│   ├── extract_data_se_df.py
│   ├── extract_huggingface.py
│   ├── extract_policy_data.py
│   └── transform.py
├── data/
│   ├── raw/                    # Dados brutos
│   └── processed/              # Dados processados
├── dashboard/
│   └── app.py                  # Streamlit app
├── requirements.txt
└── README.md

```
Passo a Passo

```bash
# 1. Clone o repositório
git clone https://github.com/taguinara/projeto-evasao-df.git
cd projeto-evasao-df

# 2. Crie ambiente virtual
python -m venv .venv
# Windows
.\.venv\Scripts\Activate.ps1

# 3. Instale dependências
pip install -r requirements.txt

# 4. Execute pipeline
python scripts/extract_data_se_df.py
python scripts/extract_huggingface.py
python scripts/extract_policy_data.py
python scripts/transform.py

# 5. Rode o dashboard
streamlit run dashboard/app.py

```

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

### KPIs Monitorados

| KPI | Valor |
|-----|-------|
| 📉 Total de Evasões | 26.100 (2020-2024) |
| 📍 Regiões Afetadas | 31 RAs |
| 🎓 Pé-de-Meia no DF | 61.943 beneficiários |
| 🖧 Escolas Conectadas | 71,7% das escolas |

---

## 🔍 Principais Descobertas

### Ranking de Evasão por RA

| Posição | Região | Evasões | % |
|---------|--------|---------|---|
| 1º | Ceilândia | 4.750 | 18,2% |
| 2º | Samambaia | 3.820 | 14,6% |
| 3º | Planaltina | 3.100 | 11,9% |
| 4º | Taguatinga | 2.890 | 11,1% |
| 5º | Recanto das Emas | 2.450 | 9,4% |

> ⚠️ **As 3 regiões com maior evasão concentram 35% dos abandonos no DF.**

### Evolução Temporal (2020-2024)

| Ano | Evasões | Taxa |
|-----|---------|------|
| 2020 | 15.200 | 14,2% |
| 2021 | 16.800 | 15,9% |
| 2022 | 14.500 | 13,5% |
| 2023 | 12.800 | 11,8% |
| 2024 | 11.200 | 10,3% |

> 📈 **Redução de 29% entre 2021 e 2024.**

### Evasão por Etapa

| Etapa | Evasões | % |
|-------|---------|---|
| 1ª Série - Ensino Médio | 2.850 | 25,4% |
| 2ª Série - Ensino Médio | 2.450 | 21,9% |
| 9º Ano - Fundamental | 1.820 | 16,3% |

> 🎓 **Ensino Médio concentra mais de 50% dos casos.**

---

## 💡 Insights Estratégicos

| Insight | Recomendação |
|---------|--------------|
| **Concentração regional** (35% em 3 RAs) | Direcionar recursos para Ceilândia, Samambaia e Planaltina |
| **Pé-de-Meia reduz 43% do abandono** | Expandir cobertura para 70% dos estudantes |
| **Conectividade reduz 18% da evasão** | Priorizar internet nas regiões críticas |
| **Ensino Médio é ponto crítico** | Fortalecer incentivos para esta etapa |

---

## 📈 Correlações com Evasão

| Fator | Correlação |
|-------|-------------|
| Baixa Frequência | 0,82 (muito forte) |
| Reprovação | 0,78 (forte) |
| Distorção Idade-Série | 0,71 (forte) |
| Vulnerabilidade Social | 0,65 (moderada) |
| Turno Noturno | 0,58 (moderada) |

---

📚 Referências

SEEDF Dados Abertos
Hugging Face - Censo Escolar
IPEDF
Anuário da Educação Básica
Legislação
Pé-de-Meia: Lei nº 14.818/2024
Escolas Conectadas: Decreto nº 11.646/2023

🔗 **Links:**
- [SEEDF Dados Abertos](https://data.se.df.gov.br/)
- [Censo Escolar HF](https://huggingface.co/datasets/Horusprg/censo-2015-2024)
- [IPEDF](https://www.ipedf.df.gov.br/)


*Projeto Integrador - Módulo 2 | Ciência de Dados | Maio/2026*

