# Registro das Alterações (P2)

## 1. Material reaproveitado
Da P1 (matrícula 241021847) foram reaproveitados, sem alteração, a planilha `Dados_Financas_P1_241021847.xlsx`, a prova em PDF/DOCX e os quatro documentos de metodologia, todos em `1_Dados_Originais_P1/`. As séries de receita e despesa nominais de 2014–2023 de Betim, Governador Valadares e Indonésia vêm dessa planilha.

## 2. O que foi refeito
- **Janela:** mantida em 2014–2023, a mais recente com dados completos para as três unidades e para o PIB municipal (o IBGE ainda não divulgou 2024).
- **PIB municipal:** extraído de `PIB_MUNICIPIOS.xlsx` (SIDRA 5938) e deflacionado pelo IPCA de dezembro, ano-base 2023.
- **Código:** `4_Codigo/analise.py` recalcula deflação, per capita, razões sobre o PIB, correlações e regressões.

## 3. Correção em relação à P1
O R² de 0,8025 (β = 133,9) de Governador Valadares na P1 resulta de regredir a receita **real** sobre o PIB **nominal**. Com o PIB também deflacionado, R² = 0,227 (p = 0,16). Para Betim, a P1 já usava PIB real (R² = 0,38), valor que se mantém. O script imprime a linha de conferência.

## 4. Pendências e riscos nos dados
- Receitas nominais de Betim em 2016, 2017 e 2018 aparecem idênticas (R$ 1,78 bi) e as de 2015 e de Valadares em 2015–2018 são números redondos: conferir no Finbra.
- 2024 não foi usado: falta PIB municipal, falta Betim e Indonésia na base, e o dado de Valadares (receita +24% nominal, despesa redonda, população 266.561 contra 282.164 em 2023) precisa de conferência. O IPCA de dez/2024 no arquivo do IPEA é 7.100,50; o CSV de Valadares usa 7.100,42.
- A coluna de PIB da Indonésia na planilha da P1 está em dólares, não em rupias; não foi usada.
- Receitas tributárias e transferências, usadas nos gráficos da P1, não estão na planilha; são necessárias para testar o efeito flypaper.
