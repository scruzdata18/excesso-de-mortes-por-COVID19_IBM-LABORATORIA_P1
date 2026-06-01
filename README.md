# Excesso de Mortes por COVID-19 na América Latina

![Status](https://img.shields.io/badge/status-concluído-brightgreen)
![Ferramenta](https://img.shields.io/badge/ferramenta-Google%20Sheets-blue)
![Programa](https://img.shields.io/badge/IBM%20%2B%20Laboratória-200h-orange)
![Área](https://img.shields.io/badge/área-saúde%20pública-lightgrey)

> **Pergunta central:** Os números oficiais de mortes por COVID-19 refletem a realidade? Uma análise comparativa entre mortes reportadas e mortes estimadas em excesso em 5 países latino-americanos.

---

## O Problema

Durante a pandemia de COVID-19, governos da América Latina reportaram oficialmente seus números de mortalidade, mas especialistas em saúde pública alertavam que esses dados podiam estar subestimados.

O **excesso de mortalidade** é uma métrica usada por epidemiologistas e organismos internacionais (OMS, IHME) para estimar o impacto real de uma crise sanitária: compara o total de mortes observadas com o que seria esperado em condições normais.

Essa diferença importa. Ela afeta decisões sobre alocação de recursos, políticas de saúde e a narrativa histórica sobre a pandemia.

---

## O que este projeto analisa

Comparação entre mortes oficialmente atribuídas ao COVID-19 e o excesso de mortalidade estimado nos 5 países da América Latina com maior número de casos, com dados normalizados por 100.000 habitantes para comparação justa entre países de tamanhos diferentes.

**Países analisados:** Brasil, México, Peru, Colômbia e Chile  
**Período:** 2020–2021  
**Ferramenta:** Google Sheets (funções QUERY, VLOOKUP, AVERAGEIFS)

> ⚠️ Os dados utilizados são fictícios e foram fornecidos para fins educacionais no contexto da certificação IBM + Laboratória. A metodologia aplicada replica abordagens reais usadas em análises epidemiológicas.

---

## Principais Achados

| País | Mortes oficiais (por 100k) | Excesso estimado (por 100k) | Diferença |
|------|---------------------------|----------------------------|-----------|
| Brasil | 279 | 352 | 73 |
| México | 213 | 523 | **310 - maior gap** |
| Peru | 601 | 697 | **96 - maior número absoluto** |
| Colômbia | 220 | 318 | 98 |
| Chile | 196 | 226 | **30 - menor gap** |

📊 O **México** apresentou a maior discrepância entre dados oficiais e excesso estimado (310 mortes/100k), sugerindo expressiva subnotificação.  
📊 O **Chile** teve os dados mais alinhados (diferença de apenas 30/100k), indicando maior capacidade de registro civil.  
📊 O **Peru** registrou o maior número absoluto de mortes em excesso por habitante (697/100k) entre os países analisados.

---

## Visualizações

**Visão geral do dataset**  
![Visão Geral](visaoGeral.png)

**Comparação: mortes oficiais vs. mortes acumuladas**  
![Comparação](comparacaoMortesMortesAcumul.png)

**Tabela comparativa por país**  
![Tabela](tabelaComparativa.png)

**Evolução temporal das mortes**  
![Série temporal](mortes_ao_longo_tempo.png)

---

## Metodologia

1. Revisão e compreensão do dataset
2. Importação e espelhamento de dados (`IMPORTRANGE`)
3. Cálculo de mortes por 100.000 habitantes (`QUERY` + `VLOOKUP`)
4. Cálculo do total acumulado por país
5. Estimativa de mortes esperadas via média histórica (`AVERAGEIFS`)
6. Cálculo do excesso: mortes observadas − mortes esperadas
7. Normalização por habitante para comparação entre países

---

## Limitações e Próximos Passos

- Dados utilizados são sintéticos (fins educacionais); análise com dados reais do SIVEP-Gripe ou DATASUS permitiria validação das hipóteses
- Expansão possível para outros países da América Latina com dados do IHME ou Our World in Data
- Migração futura para Python/Pandas para automatizar o pipeline de análise

---

## Acesse o projeto completo

📈 [Planilha de análise (Google Sheets)](https://docs.google.com/spreadsheets/d/18Mz6EnlOcX9wgjZmxvYyXZtgOg3EWn_IRkD6BbRFAWI/edit?usp=sharing)  
📹 [Vídeo de apresentação dos resultados (Loom)](https://www.loom.com/share/260b1c897b2b43a2a8327386bf373483)


---

## Contexto

Projeto desenvolvido como parte da **Certificação em Análise de Dados IBM + Laboratória** (200h), programa de formação de mulheres em tecnologia e dados na América Latina.


---

## Sobre a autora

Analista de dados com graduação em Ciência de Dados (UFMS), MBA em Data Science e Analytics (USP/ESALQ) e Mestranda em Gestão e Políticas Públicas com ênfase em Educação Profissional e Tecnológica pela FGV/EAESP (2025), com projeto de pesquisa aplicando machine learning para identificar fatores associados ao fluxo e desempenho em Itinerários Profissionais da Educação Profissional e Tecnológica em Mato Grosso do Sul.

Atua na Secretaria de Estado de Educação de MS (SED/MS), na interseção entre dados e políticas públicas educacionais de Educação Profissional e Tecnológica.

🔗 [LinkedIn](https://www.linkedin.com/in/sthefcruz18/) | [Portfólio](https://bit.ly/sthefcruz18) | [GitHub](https://github.com/sthefcruz18)
