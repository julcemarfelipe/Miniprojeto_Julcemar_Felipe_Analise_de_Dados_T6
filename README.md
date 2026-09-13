# Mini-Projeto Avaliativo — Análise Exploratória de Dados (Base Varejo)

Projeto da disciplina **Análise de Dados com Python** (Turma Analise_de_Dados_T6),
Módulo 1 - Semana 07.

**Autor:** Julcemar Justino Felipe

## Objetivo

Realizar uma Análise Exploratória de Dados (AED) sobre uma base de compras de
varejo, praticando: inspeção inicial, diagnóstico de qualidade de dados,
limpeza, validação de regras de negócio, estatística descritiva e agrupamentos.

## Arquivos do projeto

| Arquivo | Descrição |
|---|---|
| `Base_Varejo.ipynb` / `miniprojeto_varejo.py` | Script/Notebook principal, com todas as etapas da análise |
| `Base Varejo.csv` | Base de dados original (não incluída no repositório — baixe do Kaggle) |
| `df_limpo.csv` | Gerado automaticamente ao rodar o script (base já limpa, 1 linha = 1 item com `QUANTIDADE`) |
| `df_compras.csv` | Gerado automaticamente ao rodar o script (1 linha = 1 compra agregada por `CO_ID`) |

## Como rodar

1. Baixe a base `Base Varejo.csv` do Kaggle (link no enunciado do mini-projeto) e
   coloque na mesma pasta deste script/notebook.
2. Rode no terminal:
   ```bash
   python miniprojeto_varejo.py