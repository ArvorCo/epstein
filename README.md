# Investigacao Jornalistica: Caso Jeffrey Epstein

Uma investigacao jornalistica baseada em analise computacional de **6 milhoes de documentos** do caso Jeffrey Epstein.

## Fonte dos Documentos

Todos os documentos analisados foram baixados publicamente do site oficial do Departamento de Justica dos Estados Unidos:

**[justice.gov/epstein](https://www.justice.gov/usao-sdny/jeffrey-epstein-related-documents)**

Os documentos incluem:
- Depoimentos judiciais
- Emails apreendidos
- Documentos financeiros
- Depoimentos de vitimas
- Registros de voos
- Diarios pessoais

## Ferramentas de Analise

Esta investigacao utilizou as seguintes ferramentas para processar e analisar o corpus de documentos:

### Datashare + Elasticsearch
- Indexacao full-text de 384.890 documentos
- Busca semantica e highlighting
- Named Entity Recognition (NER)
- Agregacoes e estatisticas

### Neo4j
- Grafo com 1.3 milhoes de entidades
- 5.5 milhoes de relacionamentos
- Analise de redes e conexoes entre pessoas
- Identificacao de co-ocorrencias em documentos

### Python
- Scripts de queries e analise
- Processamento de resultados
- Geracao de estatisticas

## Dossies Disponiveis

| Arquivo | Descricao |
|---------|-----------|
| [INVESTIGACAO_EPSTEIN_COMPLETA.md](docs/INVESTIGACAO_EPSTEIN_COMPLETA.md) | Artigo investigativo principal |
| [dossie_brasil_rede_influencia.md](docs/dossie_brasil_rede_influencia.md) | Conexoes Brasil: rede financeira, politica e social |
| [dossie_brasil_conexoes.md](docs/dossie_brasil_conexoes.md) | Conexoes Brasil: investigacao inicial |
| [dossie_linguagem_codificada.md](docs/dossie_linguagem_codificada.md) | Investigacao de linguagem codificada (termos verificados) |
| [dossie_diarios_vitima_programa_eugenia.md](docs/dossie_diarios_vitima_programa_eugenia.md) | Diario da vitima e programa de eugenia |
| [ilha_vitimas_investigacao.md](docs/ilha_vitimas_investigacao.md) | Investigacao sobre a ilha e vitimas |
| [valdson_dossier_revisado.md](docs/valdson_dossier_revisado.md) | Dossie sobre funcionario brasileiro |

## Numeros da Investigacao

| Metrica | Total |
|---------|-------|
| Documentos analisados | 6.002.845 |
| Documentos com alegacoes de abuso sexual | 2.051 |
| Documentos sobre trafico humano | 3.032 |
| Entidades extraidas (Neo4j) | 1.306.927 |
| Relacionamentos (Neo4j) | 5.500.000+ |

## Verificacao

Todos os documentos citados podem ser verificados em:

**[justice.gov/epstein/search](https://www.justice.gov/usao-sdny/jeffrey-epstein-related-documents)**

Basta buscar pelo codigo do documento (ex: EFTA00147413).

## Aviso Legal

Esta e uma investigacao jornalistica baseada em documentos publicos. Todas as alegacoes sao citacoes diretas dos documentos judiciais e devem ser verificadas nas fontes originais.

---

*Investigacao realizada em Fevereiro de 2026*
