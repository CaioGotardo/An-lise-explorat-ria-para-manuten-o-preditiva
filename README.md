# Análise Exploratória para Manutenção Preditiva (AI4I 2020)

Análise exploratória de dados de máquinas industriais, feita em Python como Sprint 1 de um projeto de manutenção preditiva.

## Dados
- **Dataset:** AI4I 2020 Predictive Maintenance Dataset (UCI Machine Learning Repository), licença CC BY 4.0.
- **Amostra:** 150 registros sorteados de 10.000 (`df.sample(n=150, random_state=42)`).
- **Variáveis:** temperatura do ar, temperatura do processo, rotação, torque e desgaste da ferramenta.

## O que foi feito
- Média, mediana e moda
- Quartis e amplitude interquartil (IQR)
- Histogramas de cada variável
- Gráficos de dispersão e correlação de Pearson

## Principais resultados
- Torque × rotação: correlação negativa forte (r = −0,86), com relação curva.
- Temperatura do ar × temperatura do processo: correlação positiva forte (r = 0,87).
- Desgaste da ferramenta sem relação linear com as demais variáveis (|r| < 0,13).
- Outliers de rotação (~2200 rpm) e torque (> 60 Nm) seguem a tendência geral.

## Limitações
Com 150 registros, correlações próximas de zero indicam ausência de relação linear visível, não relação fraca confirmada.

## Próximos passos
Treinar um modelo de classificação para prever falhas usando a base completa, medindo precisão, recall e F1.

## Como abrir
Abra o notebook `analise_exploratoria_ai4i2020.ipynb` no GitHub ou no Google Colab.

## Referência
Matzka, S. (2020). AI4I 2020 Predictive Maintenance Dataset. UCI Machine Learning Repository.
