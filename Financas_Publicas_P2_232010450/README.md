# Finanças do Setor Público – P2

Artigo: **Quem ajusta a quem? Sincronia entre receita e despesa e sensibilidade da arrecadação ao PIB em Betim, Governador Valadares e Indonésia (2014–2023)**

Aluno: [Seu nome] – Matrícula 232010450 · UnB – Ciências Contábeis · Disciplina: Finanças do Setor Público

## Estrutura

| Pasta | Conteúdo |
|---|---|
| `1_Dados_Originais_P1/` | Material da P1 (matrícula 241021847), mantido sem alterações: planilha, prova em PDF/DOCX e documentos de metodologia. |
| `2_Dados_Brutos_Atualizados/` | Arquivos como baixados das fontes (PIB municipal SIDRA 5938, IPCA IBGE/IPEA) e a tentativa de extensão para 2024 de Governador Valadares. |
| `3_Dados_Tratados/` | Séries reais (preços de 2023) e resultados, gerados por `4_Codigo/analise.py`. |
| `4_Codigo/` | Script que reproduz todas as tabelas do artigo. |
| `5_Artigo/` | Versão final do artigo (exportar do documento para PDF ou DOCX e salvar aqui). |
| `Registro_das_Alteracoes.md` | O que foi reaproveitado, corrigido e o que ficou pendente. |

## Como reproduzir

```bash
pip install -r requirements.txt
python 4_Codigo/analise.py
```

## Fontes
Siconfi/Finbra (receitas e despesas municipais), IBGE (população e PIB municipal, Tabela 5938), IBGE/IPEA (IPCA, dez. 1993 = 100), FMI WEO e Banco Mundial (Indonésia). Detalhes em `1_Dados_Originais_P1/REFERENCIAS_FONTES_DADOS.md`.

## Base de partida
Este trabalho parte da base da avaliação P1 de Marcos Vinicius Menezes do Nascimento (matrícula 241021847): https://github.com/marcosviniciusmenezes500-commits/Financas_Publicas_P1_241021847
