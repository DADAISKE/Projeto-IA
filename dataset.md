# Dataset — Statlog (German Credit Data)

**Fonte:** UCI Machine Learning Repository — Hofmann, H. (1994). *Statlog (German Credit Data)*.
Disponível em: https://archive.ics.uci.edu/dataset/144/statlog+german+credit+data
**Licença:** Creative Commons Attribution 4.0 International (CC BY 4.0)

## Descrição breve

Base pública com **1.000 registros** de clientes de um banco alemão que solicitaram crédito
ao consumidor (pessoa física). Cada registro traz dados cadastrais/financeiros do cliente e
um rótulo indicando se ele foi um bom (`good`) ou mau (`bad`) pagador.

Utilizamos a versão simplificada do dataset original (9 variáveis preditoras, em vez das 20
da versão completa do UCI), amplamente disponibilizada em plataformas como o Kaggle.

## Variáveis

| Coluna | Descrição |
|---|---|
| Age | Idade do cliente (anos) |
| Sex | Sexo do cliente |
| Job | Nível de qualificação profissional (0 a 3) |
| Housing | Situação de moradia (own, rent, free) |
| Saving accounts | Faixa de saldo em poupança (pode estar ausente = sem conta) |
| Checking account | Faixa de saldo em conta corrente (pode estar ausente = sem conta) |
| Credit amount | Valor do crédito solicitado (marcos alemães) |
| Duration | Duração do crédito (meses) |
| Purpose | Finalidade do crédito |
| **Risk** | Variável-alvo: `good` (adimplente) ou `bad` (inadimplente) |

## Observações éticas

Dataset público e anonimizado, sem informações que identifiquem os clientes. Ainda assim,
contém dados pessoais sensíveis (situação financeira), por isso o projeto trata os princípios
da LGPD (finalidade, minimização, transparência e explicabilidade) como se aplicáveis a um
cenário real de uso, mesmo não sendo obrigatórios para esta base pública.
