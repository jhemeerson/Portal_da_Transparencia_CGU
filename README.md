# Portal_da_Transparencia_CGU

# 🇧🇷 Portal da Transparência — Análise de Riscos e Anomalias

> **Projeto de Data Analytics & Business Intelligence aplicado à análise de despesas públicas, identificação de anomalias e priorização de riscos.**

---

## 📌 Sobre o projeto

Este projeto utiliza dados do **Portal da Transparência** para construir uma visão analítica sobre transações financeiras, permitindo identificar padrões de comportamento, concentração de valores e registros que apresentam características estatisticamente atípicas.

O objetivo não é afirmar a existência de irregularidades, mas utilizar **dados, indicadores estatísticos e técnicas de análise exploratória** para direcionar a atenção dos gestores para os casos que apresentam maior potencial de investigação.

A análise transforma um grande volume de transações em uma estrutura de **priorização baseada em risco**.

---

## 📊 Dashboard

👉 [**Acessar o Relatório Interativo — Power BI**](https://app.powerbi.com/view?r=eyJrIjoiZWNiM2U5YmYtOGE3OS00YzlhLThjZTEtYjBiM2I2OTkzY2E5IiwidCI6ImY3YTVkZDQwLTZjODctNDE0Yy1hMjBlLTgxNmJiM2JjM2ZiYSJ9)

---

## 🎯 Objetivos

* Analisar o comportamento das transações financeiras.
* Identificar transações classificadas em níveis de alerta.
* Detectar **outliers financeiros** por meio de Z Score.
* Identificar concentração de valores por órgão e favorecido.
* Analisar padrões temporais de movimentação.
* Avaliar relações entre **portadores e favorecidos**.
* Apoiar a priorização de casos para investigação.
* Transformar dados financeiros em informações para **tomada de decisão**.

---

## 📊 Principais indicadores

| Indicador                       |               Resultado |
| ------------------------------- | ----------------------: |
| **Transações analisadas**       |                  48.000 |
| **Valor transacionado**         |       R$ 265,95 milhões |
| **Ticket médio**                |             R$ 5.540,62 |
| **Transações em nível normal**  |                  93,32% |
| **Transações em nível crítico** |                   4,11% |
| **Período analisado**           | 01/01/2023 — 31/12/2026 |

Os dados indicam que, embora a quantidade de transações críticas represente uma parcela relativamente pequena do universo analisado, os registros críticos podem apresentar **impacto financeiro relevante**.

Por isso, a análise considera não apenas a quantidade de alertas, mas também:

**Quantidade × Valor × Órgão × Favorecido × Portador × Tempo**

---

# 🔎 Principais insights

## 1. Baixa proporção de alertas, mas alto impacto financeiro

A maior parte das transações está classificada como normal:

* 🟢 **93,32%** — nível normal
* 🔴 **4,11%** — nível crítico
* 🟡 **2,57%** — nível moderado

Considerando as 48 mil transações analisadas, os 4,11% críticos representam aproximadamente **1.973 transações**.

Entretanto, os maiores registros críticos possuem valores elevados, chegando a aproximadamente:

* R$ 3,78 milhões
* R$ 2,16 milhões
* R$ 1,79 milhão
* R$ 1,59 milhão
* R$ 1,57 milhão

Os **10 maiores registros críticos** apresentados somam aproximadamente **R$ 18,73 milhões**, equivalente a cerca de **7% do valor total transacionado**.

### 💡 Insight

> O percentual de transações críticas é reduzido, porém os registros críticos possuem impacto financeiro relevante. A priorização deve considerar principalmente o valor financeiro associado ao alerta.

---

# 🏛️ 2. Concentração de risco por órgão

A análise demonstra concentração dos maiores valores classificados como críticos em determinados órgãos.

O **Ministério da Integração e do Desenvolvimento Regional** aparece com destaque entre os maiores valores transacionados.

Essa concentração não representa, isoladamente, uma evidência de irregularidade.

Ela representa um **sinal para priorização analítica**.

### Perguntas para investigação

* Qual percentual do valor crítico está concentrado nesse órgão?
* A concentração está relacionada a contratos ou programas específicos?
* Existem poucos favorecidos concentrando os pagamentos?
* Os valores estão concentrados em determinados períodos?
* Os mesmos favorecidos aparecem repetidamente?
* Existe concentração por unidade gestora?
* Há justificativa operacional para os valores identificados?

---

# 📈 3. Outliers financeiros

A análise de **Z Score × Valor da Transação** identificou registros significativamente distantes do comportamento predominante da base.

Entre os maiores Z Scores observados:

| Z Score aproximado |
| -----------------: |
|          **20,40** |
|              11,48 |
|               9,43 |
|               9,41 |
|               8,35 |
|               8,22 |
|               8,16 |
|               8,02 |
|               7,74 |
|               7,73 |

O maior registro apresenta aproximadamente:

**Z Score = 20,40**
**Valor ≈ R$ 3,78 milhões**

### ⚠️ Importante

Um outlier estatístico **não significa automaticamente fraude, erro ou irregularidade**.

Uma transação estatisticamente atípica pode estar relacionada a:

* Contratos de grande porte;
* Pagamentos extraordinários;
* Aquisições concentradas;
* Eventos específicos;
* Sazonalidade;
* Operações legítimas, porém incomuns.

Portanto:

> **O Z Score deve ser utilizado como mecanismo de priorização para investigação, e não como conclusão de irregularidade.**

---

# 📅 4. Forte concentração temporal

A distribuição dos valores apresenta comportamento desigual ao longo dos períodos analisados.

Entre os valores apresentados:

| Mês       | Valor aproximado |
| --------- | ---------------: |
| Janeiro   |    R$ 48 milhões |
| Fevereiro |    R$ 17 milhões |
| Março     |    R$ 20 milhões |
| Abril     |    R$ 15 milhões |
| Maio      |    R$ 17 milhões |
| Junho     |    R$ 19 milhões |
| Julho     |    R$ 21 milhões |
| Agosto    |    R$ 13 milhões |
| Setembro  |     R$ 8 milhões |
| Outubro   |     R$ 5 milhões |
| Novembro  |    R$ 18 milhões |
| Dezembro  |    R$ 61 milhões |

**Janeiro + Dezembro ≈ R$ 109 milhões**

Isso representa aproximadamente **41% do valor total apresentado**.

### 💡 Insight

> A distribuição temporal dos pagamentos não é homogênea. Janeiro e dezembro concentram aproximadamente 41% do valor apresentado, indicando a necessidade de investigar os fatores operacionais, orçamentários e contratuais associados a esses picos.

### 🔍 Cruzamentos recomendados

Os períodos de maior concentração podem ser cruzados com:

* Órgão;
* Favorecido;
* Natureza da despesa;
* Contrato;
* Empenho;
* Ação orçamentária;
* Unidade gestora;
* Nível de alerta.

---

# 👥 5. Concentração entre favorecidos

A análise também demonstra concentração financeira entre determinados favorecidos.

Entre os maiores valores apresentados:

* R$ 8,31 milhões
* R$ 6,99 milhões
* R$ 6,70 milhões
* R$ 5,87 milhões
* R$ 5,47 milhões
* R$ 4,58 milhões
* R$ 3,96 milhões
* R$ 3,78 milhões
* R$ 3,30 milhões
* R$ 3,02 milhões

Os **10 maiores blocos** representam aproximadamente:

**R$ 51,98 milhões**

ou cerca de:

**19,5% do valor total transacionado.**

### 💡 Insight

> A distribuição dos recursos apresenta concentração significativa em um grupo relativamente pequeno de favorecidos. Essa concentração deve ser analisada considerando contratos, volume de serviços, características dos fornecedores e recorrência dos pagamentos.

---

# 🔗 6. Relação entre portador e favorecido

A análise de relacionamento permite observar padrões que não seriam facilmente identificados analisando apenas uma transação individual.

O relacionamento:

```text
PORTADOR
    │
    ├── Transações
    │
    ▼
FAVORECIDO
    │
    └── Valor financeiro
```

permite identificar:

* Portadores com grande volume de transações;
* Favorecidos recorrentes;
* Concentração financeira;
* Relações recorrentes;
* Padrões de comportamento.

### 📌 Indicadores recomendados

| Indicador                       | Objetivo                             |
| ------------------------------- | ------------------------------------ |
| Nº de transações por portador   | Identificar concentração             |
| Nº de favorecidos por portador  | Avaliar diversidade                  |
| Valor total por portador        | Medir exposição financeira           |
| Ticket médio por portador       | Identificar comportamento financeiro |
| Nº de portadores por favorecido | Identificar concentração             |
| Valor por favorecido            | Medir concentração                   |
| % crítico por portador          | Priorizar análise                    |
| % crítico por favorecido        | Priorizar análise                    |
| Z Score médio/máximo            | Medir anomalia                       |

---

# 🔐 7. Qualidade e completude da informação

A análise apresenta categorias como:

* **SIGILOSO — R$ 8,31 milhões**
* **SEM INFORMAÇÃO — R$ 4,58 milhões**

Essas categorias não representam necessariamente um problema nos dados.

Informações podem possuir restrições legais ou características específicas de divulgação.

Porém, do ponto de vista analítico, é importante diferenciar:

```text
Risco da transação
        ≠
Risco da qualidade da informação
```

### 📊 KPI recomendado

**Índice de Completude**

```text
% de transações com informação completa
```

Também pode ser utilizado:

```text
Valor financeiro sem informação
──────────────────────────────── × 100
Valor financeiro total
```

---

# 🚨 8. Priorização baseada em risco

O principal potencial do projeto está em transformar o dashboard em uma ferramenta de **inteligência analítica para controle**.

A lógica proposta é:

```text
┌───────────────────────┐
│ 1. UNIVERSO           │
│ 48.000 transações     │
└───────────┬───────────┘
            ↓
┌───────────────────────┐
│ 2. FILTRAGEM          │
│ Transações com alerta │
└───────────┬───────────┘
            ↓
┌───────────────────────┐
│ 3. PRIORIZAÇÃO        │
│ Valor + Z Score       │
└───────────┬───────────┘
            ↓
┌───────────────────────┐
│ 4. INVESTIGAÇÃO       │
│ Órgão + Favorecido    │
│ + Portador + Histórico│
│ + Documentos          │
└───────────────────────┘
```

Essa abordagem permite sair de uma análise baseada apenas em volume e direcionar a atenção para as combinações com maior potencial de relevância.

---

# 🎯 Matriz de priorização analítica

Uma evolução proposta para o projeto é a criação de um **Índice de Prioridade Analítica**.

> O índice deve ser interpretado como mecanismo de priorização, e não como conclusão de irregularidade.

| Critério           | Pergunta                                            |
| ------------------ | --------------------------------------------------- |
| **Valor**          | A transação possui impacto financeiro elevado?      |
| **Z Score**        | Está distante do comportamento esperado?            |
| **Alerta**         | Foi classificada como crítica?                      |
| **Concentração**   | O favorecido recebe parcela relevante dos recursos? |
| **Recorrência**    | Existem muitos pagamentos semelhantes?              |
| **Temporalidade**  | Ocorre em período atípico?                          |
| **Relacionamento** | Existe concentração entre portador e favorecido?    |
| **Histórico**      | O comportamento se repete?                          |

O resultado pode gerar uma **fila de análise**, em vez de simplesmente ordenar as transações pelo maior valor.

---

# 📊 Visão conceitual da solução

```text
                 DADOS FINANCEIROS
                        │
                        ▼
              ┌───────────────────┐
              │ 48.000 transações │
              └─────────┬─────────┘
                        │
          ┌─────────────┼─────────────┐
          ▼             ▼             ▼
       ALERTAS       Z SCORE      CONCENTRAÇÃO
          │             │             │
          └─────────────┼─────────────┘
                        ▼
               ANÁLISE DE RISCO
                        │
                        ▼
             PRIORIZAÇÃO ANALÍTICA
                        │
                        ▼
               INVESTIGAÇÃO
                        │
                        ▼
       CONTRATOS / EMPENHOS / PAGAMENTOS
```

---

# 💼 Valor para o negócio

O projeto demonstra como uma solução de **Business Intelligence e Data Analytics** pode apoiar gestores na tomada de decisão.

### Benefícios

* 🔎 Identificação de padrões atípicos;
* 🎯 Priorização de análises;
* 💰 Foco em maior impacto financeiro;
* 📊 Monitoramento de indicadores;
* 🏛️ Análise por órgão;
* 👥 Análise por favorecido;
* 🔗 Identificação de relacionamentos;
* 📅 Identificação de padrões temporais;
* ⚠️ Apoio à gestão baseada em risco.

---

# 🚀 Próximos passos

Para evoluir o projeto, são recomendadas as seguintes funcionalidades:

### KPIs executivos

1. **Valor em Alertas Críticos**
2. **% do Valor sob Alerta**
3. **Quantidade de Transações Críticas**
4. **Maior Z Score**
5. **Valor Concentrado nos 10 Maiores Favorecidos**

### Nova página: `Prioridade de Análise`

Criar uma tabela com:

| Prioridade | Órgão | Favorecido | Valor | Z Score | Alerta | Data |
| ---------- | ----- | ---------- | ----: | ------: | ------ | ---- |

Ao selecionar uma transação, permitir explorar:

```text
Transação
    │
    ├── Empenho
    │
    ├── Liquidação
    │
    ├── Pagamento
    │
    ├── Favorecido
    │
    ├── Órgão
    │
    └── Contrato
```

Essa evolução aproxima o dashboard de uma ferramenta de **auditoria orientada por dados**.

---

# 🧠 Storytelling executivo

A narrativa do projeto pode ser apresentada seguindo a sequência:

```text
UNIVERSO
   ↓
CONCENTRAÇÃO
   ↓
ANOMALIAS
   ↓
RISCO FINANCEIRO
   ↓
RELAÇÕES PORTADOR × FAVORECIDO
   ↓
CASOS PRIORITÁRIOS
   ↓
INVESTIGAÇÃO DOCUMENTAL
```

Essa estrutura transforma os dashboards em uma narrativa orientada à **tomada de decisão**, e não apenas à visualização de dados.

---

# ⚠️ Considerações importantes

Os indicadores de alerta e os outliers apresentados neste projeto devem ser interpretados como **mecanismos de priorização analítica**.

Um alerta ou um Z Score elevado, isoladamente, **não comprova fraude, erro ou irregularidade**.

A validação deve considerar informações complementares, como:

* Contratos;
* Empenhos;
* Liquidações;
* Pagamentos;
* Documentos;
* Histórico;
* Contexto operacional.

> **O objetivo da análise é direcionar a investigação para onde os dados indicam maior potencial de relevância.**

---

# 🛠️ Tecnologias

**Business Intelligence**

* Power BI
* DAX
* Power Query

**Data Analytics**

* Análise exploratória de dados
* Estatística
* Z Score
* Análise de outliers
* Análise de concentração
* Análise temporal

**Data Source**

* Portal da Transparência
* Dados de execução de despesas e favorecidos

---

# 📌 Conclusão

O projeto demonstra uma aplicação prática de **Data Analytics + Business Intelligence** para transformar um grande volume de dados financeiros em informações direcionadas à tomada de decisão.

Os principais achados indicam:

* **48 mil transações analisadas**;
* **R$ 265,95 milhões movimentados**;
* **4,11% de transações em nível crítico**;
* Forte concentração dos maiores valores críticos em determinados órgãos;
* Existência de **outliers financeiros relevantes**;
* Concentração temporal significativa;
* Concentração de recursos entre determinados favorecidos;
* Relações recorrentes entre portadores e favorecidos.

O principal resultado do projeto é a mudança de uma abordagem puramente descritiva para uma abordagem de **priorização baseada em risco**, permitindo que gestores direcionem esforços para os casos que combinam maior impacto financeiro, anomalia estatística, concentração e recorrência.

---

# 👨‍💻 Autor

**Jhemerson Oliveira**

**Analista de Dados | Business Intelligence**

🔗 [**Portfólio**](https://portfolio-jhemerson-oliveira.lovable.app/)

