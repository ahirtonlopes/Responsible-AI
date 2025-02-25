# Responsible AI - Hello World with AIF360

Este repositório contém um exemplo simples de Responsible AI utilizando a biblioteca AIF360 (AI Fairness 360) da IBM. O exemplo utiliza a base de dados COMPAS, que é comumente usada para análise de viés e fairness em modelos preditivos, especialmente em sistemas de justiça criminal.

# Objetivo

Este projeto tem como objetivo demonstrar como usar a biblioteca AIF360 para avaliar e mitigar possíveis vieses em um modelo de aprendizado de máquina. O exemplo fornecido segue a abordagem "Hello World" da Responsible AI, usando a base de dados COMPAS.

## Base de Dados COMPAS

A base de dados COMPAS (Correctional Offender Management Profiling for Alternative Sanctions) contém informações sobre indivíduos envolvidos no sistema judicial dos EUA, incluindo características demográficas, histórico criminal e pontuações de risco. O objetivo é prever o risco de reincidência.

## Passos do Exemplo

- Carregamento e preparação dos dados:

O exemplo começa com o carregamento da base de dados COMPAS.
Realiza-se um pré-processamento, incluindo a conversão das variáveis categóricas em numéricas e a normalização das variáveis.

- Treinamento do modelo:

Um modelo simples de aprendizado supervisionado é treinado para prever a reincidência com base nos dados.

- Avaliação de fairness:

Utilizando a biblioteca AIF360, avaliamos a equidade do modelo, identificando possíveis vieses com relação a diferentes grupos (como raça e gênero).
Vários indicadores de fairness, como Disparate Impact, Statistical Parity e Equal Opportunity, são calculados.

- Mitigação de viés:

Após avaliar os vieses, é possível aplicar técnicas de mitigação (como o Reweighing ou Disparate Impact Removal) para melhorar a equidade do modelo.

## Exemplos de Métricas de Fairness

No notebook, você encontrará exemplos de como calcular as seguintes métricas de fairness usando AIF360:

- Disparate Impact: Mede o impacto desproporcional de um modelo em diferentes grupos.
- Statistical Parity: Compara as taxas de resultados positivos entre grupos sensíveis.
- Equal Opportunity: Compara a taxa de verdadeiros positivos entre os grupos.

## Licença

Este projeto está licenciado sob a licença MIT - veja o arquivo LICENSE para mais detalhes
