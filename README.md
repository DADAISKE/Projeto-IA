# CredScore AI: Decifrando o Risco de Crédito

Projeto da disciplina de Inteligência Artificial (7º CC) — Faculdade de Computação e Informática, Universidade Presbiteriana Mackenzie.

## Integrantes

| Nome | RA |
|---|---|
| Rodrigo Daiske Uehara | 10440295 |

## Sobre o projeto

O objetivo é comparar modelos de aprendizado de máquina (Regressão Logística, Random Forest e XGBoost) para prever o risco de inadimplência de clientes que pedem crédito ao consumidor, construindo um sistema de *credit scoring* preciso e transparente. A ideia é ajudar na inclusão financeira e diminuir bem os erros nas decisões de crédito, avaliando desempenho e equidade entre grupos de clientes (sexo e faixa etária) — não apenas presumindo esses ganhos.

O projeto está alinhado aos Objetivos de Desenvolvimento Sustentável (ODS):
- **ODS 8** – Trabalho Decente e Crescimento Econômico
- **ODS 10** – Redução das Desigualdades

## Dataset

[Statlog (German Credit Data)](https://archive.ics.uci.edu/dataset/144/statlog+german+credit+data) (Hofmann, 1994), UCI Machine Learning Repository, licenciado sob CC BY 4.0. 1.000 registros de clientes, 9 variáveis preditoras + variável-alvo `Risk` (bom/mau pagador). Descrição completa em [`README_dataset.md`](README_dataset.md).

## Estrutura do repositório

```
├── README.md                          # este arquivo
├── dataset.md                  # descrição do dataset
├── german_credit_data.csv             # dataset utilizado
├── artigo_parcial_credscoreai.docx    # artigo parcial (N1)
└── 01_analise_exploratoria.ipynb      # notebook com a análise exploratória e preparação dos dados
```

## Status do projeto

- [x] **N1 — Primeiro Bimestre**: proposta refinada, análise exploratória dos dados, definição do protocolo experimental e artigo parcial.
- [ ] **N2 — Segundo Bimestre**: treinamento e comparação dos modelos (Regressão Logística, Random Forest, XGBoost), aplicação do SHAP (XAI), avaliação de equidade entre grupos, artigo final e vídeo de apresentação.

## Metodologia (resumo)

1. Análise exploratória e preparação dos dados (concluído — ver notebook).
2. Treino dos modelos com validação cruzada estratificada.
3. Avaliação com F1-score, recall da classe inadimplente, PR-AUC, matriz de confusão e calibração.
4. Explicabilidade do melhor modelo com SHAP.
5. Avaliação de equidade entre sexo e faixa etária.
6. Discussão crítica dos resultados, limitações e riscos éticos (LGPD, viés, explicabilidade x discriminação).

## Aspectos éticos

Dataset público e anonimizado, sem necessidade de submissão a Conselho de Ética em Pesquisa. Ainda assim, o projeto discute os princípios da LGPD (finalidade, minimização, transparência e direito à revisão de decisões automatizadas — art. 20) como se aplicariam a um sistema real, e trata desempenho e equidade como avaliações separadas, já que explicabilidade não garante ausência de discriminação.
