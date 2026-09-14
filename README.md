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
| `Base_Varejo.ipynb` | Notebook principal, com todas as etapas da análise (Sprints 1 a 6) |
| `Base Varejo.csv` | Base de dados original (não incluída no repositório — baixe do Kaggle) |
| `df_limpo.csv` | Gerado automaticamente ao rodar o notebook (base limpa, 1 linha = 1 item, com `QUANTIDADE`) |
| `df_compras.csv` | Gerado automaticamente ao rodar o notebook (1 linha = 1 compra, agregada por `CO_ID`) |
| `vendas_anim.gif` | Gerado automaticamente ao rodar o notebook (animação das vendas mês a mês) |
| `figuras/` | Gerado automaticamente ao rodar o notebook (donut, boxplot e heatmap ano × mês, em `.png`) |
| `README_Julcemar_Felipe_Analise_de_Dados_T.md` | Documentação detalhada: pipeline por sprint, todas as visualizações e a reflexão teórica |

## Como rodar

1. Baixe a base `Base Varejo.csv` no Kaggle:
   <https://www.kaggle.com/datasets/namespaiva/base-varejo/data>
2. Coloque o `Base Varejo.csv` na mesma pasta do notebook `Base_Varejo.ipynb`.
3. Abra o notebook no **Google Colab** (upload do `.ipynb` + do `.csv`) ou no
   **VSCode** (com a extensão Jupyter) e rode todas as células, em ordem.
4. O relatório da análise aparece na saída de cada célula. Ao final, o
   notebook gera `df_limpo.csv`, `df_compras.csv`, `vendas_anim.gif` e a
   pasta `figuras/` na mesma pasta do projeto.

### Dependências

```bash
pip install pandas numpy matplotlib pillow
```

## Principais insights (resumo)

- A base cobre 18.471 compras de 1.000 clientes distintos, entre 04/01/2019 e 08/12/2022.
- **ALIMENTOS** é a categoria líder, com 434.767 unidades — bem acima de HIGIENE (155.574) e LIMPEZA (145.754).
- O gênero **F** concentra um pouco mais de compras que o **M** (9.615 vs. 8.856), sem indicar um público dominante.
- Um único produto (`PR_ID` 107, sem cadastro) responde por 100% dos 3.650 registros com categoria `"#N/D"`.
- As 96.553 linhas duplicadas viraram a coluna `QUANTIDADE`, em vez de serem descartadas.
- O número médio de filhos por cliente é 1,14 (mediana 0); o segmento **C** tem a maior média (1,18).

Para o pipeline completo por sprint, o dicionário de dados e a reflexão
teórica sobre ETL e qualidade de dados, veja o
[README_Julcemar_Felipe_Analise_de_Dados_T.md](./README_Julcemar_Felipe_Analise_de_Dados_T.md).
