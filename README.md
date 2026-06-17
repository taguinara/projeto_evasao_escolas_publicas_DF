
# 📊 Evasão Escolar — Dashboard (Distrito Federal)

Este repositório contém o pipeline e o dashboard interativo desenvolvidos para o Projeto Integrador de Ciência de Dados — análise da evasão escolar nas escolas públicas do Distrito Federal (2015–2024).

Link do app dashboard (Streamlit cloud): https://projetoevasaoescolaspublicasdf-projeto.streamlit.app/

## Conteúdo

- `scripts/` — scripts de extração e transformação (ETL)
- `data/raw/` — dados brutos (não comitados)
- `data/processed/` — dados processados usados pelo dashboard
- `dashboard/app.py` — aplicação Streamlit
- `requirements.txt` — dependências Python

## Rápido (clone, setup e execução)

1. Clone o repositório

```bash
git clone https://github.com/taguinara/projeto-evasao-escolas_publicas_DF.git
cd projeto_evasao_escolas_publicas_DF
```

2. Crie e ative um ambiente virtual

Windows PowerShell:
```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

3. Instale dependências

```powershell
pip install -r requirements.txt
```

4. Execute o pipeline (gera `data/processed/`)

```powershell
python scripts/extract_data_se_df.py
python scripts/extract_huggingface.py --state DF
python scripts/extract_policy_data.py
python scripts/transform.py
```

5. Rode o dashboard localmente

```powershell
streamlit run dashboard/app.py
```

6. (Opcional) Rode o DAG do Airflow para automação da pipeline

```powershell
python evasao_escolar_dag.py
```

## Contribuições

Abra uma issue para bugs ou sugestões. Pull requests são bem-vindos.

---

_Projeto Integrador — Ciência de Dados | Junho/2026_

