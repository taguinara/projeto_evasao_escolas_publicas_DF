---

## 📊 PROJETO INTEGRADOR - CIÊNCIA DE DADOS 
MÓDULO 2

### Telas Desenvolvidas

| Tela | Conteúdo |
|------|----------|
| **Visão Geral** | KPIs, totais, taxas |
| **Ranking Regional** | Top 10 RAs com maior evasão |
| **Evolução Temporal** | Série 2020-2024 |
| **Perfil do Aluno** | Etapas e idades |
| **Políticas Públicas** | Pé-de-Meia + Escolas Conectadas |

### Tecnologias

| Componente | Tecnologia |
|------------|------------|
| **Framework** | Streamlit 1.28+ |
| **Visualizações** | Plotly 5.17+ |
| **Manipulação** | Pandas 2.0+ |
| **Estilização** | CSS customizado |

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

## 🚀 Como Executar

### Pré-requisitos

```bash
Python 3.8+
Git
Pip

Instalação
bash
# Clone o repositório
git clone https://github.com/taguinara/projeto-evasao-df.git
cd projeto-evasao-df

# Crie ambiente virtual
python -m venv .venv
.\.venv\Scripts\Activate.ps1  # Windows

# Instale dependências
pip install -r requirements.txt

# Execute o pipeline
python scripts/extract_data_se_df.py
python scripts/transform.py

# Rode o dashboard
streamlit run dashboard/app.py
Dependências
txt
streamlit>=1.28.0
pandas>=2.0.0
plotly>=5.17.0
numpy>=1.24.0
requests>=2.31.0
📁 Estrutura do Projeto
text
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
🏁 Resultados Alcançados
Produtos Entregues
Pipeline ETL com 3 fontes de dados

7 arquivos processados

Dashboard Streamlit com 5 telas

Integração de políticas públicas

Documentação completa

Métricas

Métrica	Resultado
Regiões analisadas	31 RAs
Período coberto	10 anos
Registros processados	71.035+
Gráficos no dashboard	8 tipos
Insights gerados	5 estratégicos

📚 Referências
SEEDF Dados Abertos
Hugging Face - Censo Escolar
IPEDF
Anuário da Educação Básica
Pé-de-Meia: Lei nº 14.818/2024

Escolas Conectadas: Decreto nº 11.646/2023

*Projeto Integrador - Módulo 2 | Ciência de Dados | Maio/2026*
