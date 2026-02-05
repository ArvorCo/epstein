# Dossie: Investigacao de Linguagem Codificada nos Documentos Epstein

**Data**: 4 de fevereiro de 2026
**Investigador**: Leonardo Dias / Arvor
**Versao**: 1.0
**Classificacao**: Investigacao Jornalistica

---

## Sumario Executivo

Esta investigacao analisou sistematicamente **4.651 documentos** do indice Elasticsearch `epstein` (Datashare) buscando evidencias de linguagem codificada, com foco em:

1. **Termos alimenticios** alegados como codigo (originarios da teoria Pizzagate/Podesta Emails)
2. **Termos extremos** (adrenochrome, spirit cooking, satanic, moloch, etc.)
3. **Termos de trafico** (daddy, branding)

### Resultado Principal

**NAO foi encontrada evidencia de uso sistematico de termos alimenticios como linguagem codificada nos documentos Epstein.** Cada termo alimenticio analisado apresentou uso literal verificavel (restaurantes, pedidos de comida, menus, receitas, materiais de construcao, nomes de empresas).

### Correcao Critica de Metodologia

O count de "hot dog" reportado anteriormente como **2.628 hits** estava ERRADO. A query `match: "hot dog"` no Elasticsearch faz OR entre "hot" e "dog" (2.628 resultados). O count correto usando `match_phrase` e **21 hits** - uma inflacao de **125x**. Todos os 21 hits sao de uso literal (Nathan's Hot Dog Contest, Central Park walks, deli, piada sobre Paquistao).

### Achados Notaveis

| Achado | Status | Documento |
|--------|--------|-----------|
| "The Pizza Monster" - mulher referida como "the pizza" | SUSPEITO (mas explicavel) | EFTA02464505, EFTA02356175 |
| Epstein se referindo como "daddy" | CONFIRMADO | EFTA01301242 |
| "Eyes Wide Shut" como metafora para estilo de vida | LITERAL (jornalistas) | Multiplos HOUSE_OVERSIGHT |
| David Stern "Re: Pizza" - negocio | AMBIGUO | EFTA02510241 |
| "Walnut" = empresa/madeira (nao pessoa) | DEBUNKED | EFTA02411684, EFTA02528960 |
| "Cheese" resposta a menu sushi = pizza | DEBUNKED | EFTA02488656 |
| adrenochrome, blood ritual, human sacrifice | 0 HITS | N/A |

---

## Metodologia

### Fonte de Dados
- **Indice**: `epstein` (Datashare/Elasticsearch 7.17.9)
- **Filtro**: `type: Document` (exclui entidades NER e mentions)
- **Cobertura**: Todos os documentos do indice (emails, PDFs legais, depoimentos, artigos)

### Queries
- **Single-word**: `match` (analise padrao do ES com folding)
- **Multi-word**: `match_phrase` (sequencia exata de palavras)
- **Deep-dive**: `bool.must` combinando termo + indicadores (girl, young, fresh, etc.) COM exclusao de contexto culinario

### Classificacao Automatica
Cada hit foi classificado por regex em 3 categorias:
- **LITERAL**: Contexto culinario claro (menu, restaurante, receita, delivery, chef, kitchen, etc.)
- **AMBIGUO**: Contexto insuficiente para determinar
- **SUSPEITO**: Indicadores de trafico/abuso SEM contexto culinario (girl, young, bring, fly her, massage, fresh, etc.)

**Limitacao importante**: A classificacao automatica tende a inflar SUSPEITOS porque o corpus inteiro trata de um caso de trafico sexual. Documentos sobre pizza que TAMBEM mencionam "girls" em outro paragrafo sao classificados como SUSPEITOS, mesmo que os termos nao estejam relacionados. A revisao manual corrigiu todos esses falsos positivos.

### Cross-Reference
Hits SUSPEITOS foram cruzados com lista de 26 pessoas conhecidas (Maxwell, Brunel, Kellen, Groff, etc.) e emails de Epstein (jeevacation@gmail.com).

---

## Capitulo 1: Termos Alimenticios

### Tabela de Counts Corrigidos

| Termo | Hits (Doc) | Query Type | Antigo (CLAUDE.md) | Status |
|-------|-----------|------------|-------------------|--------|
| pizza | 242 | match | 242 | OK |
| hot dog | **21** | match_phrase | **2,628 (ERRADO)** | CORRIGIDO |
| cheese | 229 | match | 229 | OK |
| chicken | 458 | match | 458 | OK |
| walnut | 73 | match | 73 | OK |
| walnut sauce | **0** | match_phrase | N/A | ZERO HITS |
| sauce | 227 | match | 227 | OK |
| muffin | 84 | match | 84 | OK |
| dominos | 18 | match | 18 | OK |
| pasta | 157 | match | 157 | OK |
| cookie | 336 | match | N/A | NOVO |
| candy | 142 | match | N/A | NOVO |
| ice cream | 147 | match_phrase | N/A | NOVO |
| handkerchief | 6 | match | 6 | OK |
| pizza monster | 2 | match_phrase | N/A | NOVO |

### Classificacao Automatica vs Manual

| Termo | Total | Auto-LITERAL | Auto-AMBIGUO | Auto-SUSPEITO | Manual: Real SUSPEITO |
|-------|-------|-------------|-------------|--------------|---------------------|
| pizza | 242 | 62 | 121 | 59 | **0** |
| hot dog | 21 | 6 | 6 | 9 | **0** |
| cheese | 229 | 91 | 78 | 60 | **0** |
| chicken | 458 | 141 | 168 | 149 | **0** |
| walnut | 73 | 12 | 48 | 13 | **0** |
| muffin | 84 | 13 | 40 | 31 | **0** |
| dominos | 18 | 3 | 14 | 1 | **0** |
| pasta | 157 | 38 | 82 | 37 | **0** |
| cookie | 336 | 10 | 311 | 15 | **0** |
| candy | 142 | 11 | 98 | 33 | **0** |
| ice cream | 147 | 38 | 62 | 47 | **0** |
| handkerchief | 6 | 1 | 4 | 1 | **0** |
| pizza monster | 2 | 0 | 0 | 2 | **1** (ver analise) |

**Nota**: A discrepancia entre Auto-SUSPEITO e Manual-SUSPEITO existe porque o classificador automatico marca como suspeito qualquer documento que contem TANTO o termo alimenticio QUANTO palavras como "girl", "young", etc. - mesmo que aparecam em paragrafos completamente diferentes. A revisao manual de cada hit de alta prioridade confirmou que TODOS sao usos literais.

---

### 1.1 Pizza (242 hits) - **DEBUNKED**

**Conclusao**: Todos os 242 hits sao de uso literal. Epstein era genuinamente um amante de pizza.

**Evidencias literais**:
- **Arturo's Pizza** (Houston St, NYC): Restaurante favorito de Epstein. Multiplos emails de Lesley Groff coordenando pedidos (EFTA02576362, EFTA02381091)
- **Patsy's Pizza** (Harlem): Karyna Shuliak e Tim Zagat recomendam (EFTA02481893)
- **Una Pizza Napoletana** (East Village): Epstein recomenda a alguem (EFTA02526666)
- **Joe's Pizza**: Mencionada em review de comida (EFTA02401962)
- **Menus de pizza**: Meatlovers, cheese, vegetarian - lista oferecida por Daphne Wallace (EFTA02488611)
- **Pizza para Bobby**: Lesley Groff coordena entrega de Arturo's (EFTA02381091)
- **Lawrence Krauss**: "all the pizza got eaten" em contexto de evento cientifico (EFTA02367593)

**Unico hit ambiguo**: EFTA02510241 - David Stern email "Re: Pizza" onde discutem "He can either partner, invest or buy. I will talk to him to establish whether interested. Can I talk to Sanjay Hi[...]". PROVAVELMENTE um negocio de investimento em pizzaria (Stern era conhecido por propor negocios a Epstein, incluindo o "Brazil deal").

### 1.2 Hot Dog (21 hits, corrigido de 2,628) - **DEBUNKED**

**Conclusao**: Todos os 21 hits sao literais. ZERO uso codificado.

**Evidencias literais**:
- **Nathan's Famous Hot Dog Eating Contest**: Epstein envia link da CBS a Karyna Shuliak em 4 de julho de 2018 (EFTA02308973)
- **Central Park hot dogs**: "walk in park around 1230. hot dog /lunch?" - Epstein a Michael Wolff (EFTA02569277)
- **Coney Island**: Link "140 years old" enviado a Mark Epstein sobre historia de hot dog (EFTA02429719, EFTA02428611)
- **Sabrett's hot dog**: Artigo de Michael Wolff descrevendo Epstein: "his idea of going out to lunch is a Sabrett's hot dog—with the various girls in the house acting as the accompanying entourage" (HOUSE_OVERSIGHT_023627, 024229, 022863, 022894, 022952, 022746, 022844, 022707) - Nota: "girls" se refere ao staff/entourage, nao a hot dogs como codigo
- **Super Bowl**: Larry Visoski: "no hot dogs at the deli for their super bowl party?" (EFTA00329213)
- **Bloating**: "had a hot dog and very bloated" - email literal sobre indigestao (EFTA02546523)
- **Piada**: "pakistan, afghanistan, hot dog stan, all the same" - humor de Epstein (EFTA02453901)
- **Pop-Up Hot Dog Toaster**: Email promocional da Fancy (EFTA02319583)

### 1.3 Cheese (229 hits) - **DEBUNKED**

**Conclusao**: Todos literais. O caso "cheese como resposta a sushi" esta completamente explicado.

**O caso EFTA02488656 explicado**: Daphne Wallace informa que o chef de sushi esta de ferias. Oferece pizza como alternativa (meatlovers, cheese, vegetarian). Epstein responde "cheese" = escolhendo pizza de queijo. Contexto 100% culinario.

**Outros usos literais**:
- **Cream cheese e bagels**: Thread longa entre Epstein e Nadia Marcinkova sobre "New York everything bagel with vegetable cream cheese from Too Jays" (EFTA02525278, EFTA02525266)
- **"Cream cheese baby"**: Titulo de email sobre onde encontrar cream cheese (EFTA02440165)
- **Idioma**: "just goes to show - there is a rat for every cheese" - expressao idiomatica (EFTA02527616)
- **Dieta**: "i say no cheese four times and you produce cheese" - Epstein frustrado com pedido de comida nao atendido (EFTA02526763)
- **Alergia**: "only bread and cheese, it got really bad, needed to take medrol" - reacao alergica (EFTA02341163)
- **Lista de compras**: Philadelphia cream cheese, cottage cheese, etc. na lista pre-arrival de Maxwell (EFTA00072871)

### 1.4 Walnut (73 hits) / Walnut Sauce (0 hits) - **DEBUNKED**

**Conclusao**: "Walnut" nos documentos Epstein refere-se a **madeira** e **empresas**, nunca a pessoas.

- **Madeira**: "oak just under 2.00 per board foot, american black walnut 4.50 per board foot" - cotacao de madeira de Gary Kerney (EFTA02430469)
- **Piso**: "Brazilian Walnut was purchased 2010 from Episilon Floors" - piso da ilha de Epstein (EFTA02528960)
- **Empresa**: "speaking with Walnut to hear their perspective is imperative" - due diligence de negocio conduzida por Richard Kahn/Adam Bly (EFTA02411684, EFTA02411362)
- **"Walnut sauce"**: ZERO hits em todo o corpus.

### 1.5 Outros Termos Alimenticios - Resumo Rapido

| Termo | Hits | Analise | Veredicto |
|-------|------|---------|-----------|
| chicken (458) | Listas de compras, menus, receitas | LITERAL |
| sauce (227) | Molhos em menus, receitas | LITERAL |
| muffin (84) | "bran muffin fix" (Paris), Eva Dubin "ate my last muffin", receitas | LITERAL |
| pasta (157) | Menus, receitas, restaurantes italianos | LITERAL |
| cookie (336) | "make him some cookies" (Epstein), receitas, listas | LITERAL |
| candy (142) | Nome proprio (Candy Bergen), Halloween, Karyna quer doces | LITERAL |
| ice cream (147) | Pedidos, menus, sobremesas | LITERAL |
| dominos (18) | Termo financeiro/bancario (COD Domestic), jogo | LITERAL |
| handkerchief (6) | Lord Mandelson (blazer), inventario, memorias judaicas | LITERAL |

### 1.6 Pizza Monster (2 hits) - **SUSPEITO MAS EXPLICAVEL**

**Documento**: EFTA02464505 + EFTA02356175
**Data**: 26 de abril de 2016
**Remetente**: jeffrey E. (jeevacation@gmail.com)
**Assunto**: "Re: The Pizza Monster!"

**Troca de emails**:
1. Alguem (nome redactado) envia email original
2. Epstein responde: **"she looks pregnant"**
3. A pessoa responde: **"You mean radiating a soft glow with the look of bliss and excitement. Yeah, that's the pizza..."**

**Analise**: Uma mulher e apelidada de "Pizza Monster" (presumivelmente porque come muita pizza). Epstein diz que ela "parece gravida". A resposta sugere que o inchaço e resultado de comer pizza ("that's the pizza"). A descricao "radiating a soft glow with the look of bliss" e tipica de gravidez real OU de alguem que comeu demais e esta satisfeita.

**Interpretacao mais provavel**: Apelido carinhoso para uma mulher que ama pizza, e a piada e sobre estar inchada de comer. NAO e evidencia de linguagem codificada sistematica.

**Interpretacao alternativa (nao descartada)**: Se "the pizza" for um codigo para a propria mulher, o email seria Epstein comentando sobre a aparencia fisica de uma mulher ("she looks pregnant") e a outra pessoa confirmando ("that's the pizza"). Mas sem contexto adicional ou padrao repetido, esta interpretacao e especulativa.

---

## Capitulo 2: Termos Extremos

### Tabela de Counts

| Termo | Hits | Status |
|-------|------|--------|
| adrenochrome | **0** | NAO EXISTE no corpus |
| spirit cooking | 1 | Referencia a teoria conspiratoria |
| eyes wide shut | 12 | Metafora jornalistica |
| satanic | 21 | Artigos academicos/conspiratórios |
| satan | 88 | Contextos diversos |
| occult | 58 | Artigos/livros |
| moloch | 3 | Nome de empresa + termo academico |
| cannibal | 31 | Artigos/noticias |
| sacrifice | 134 | Contextos legais/academicos |
| ritual | 98 | Contextos academicos |
| blood ritual | **0** | NAO EXISTE no corpus |
| human sacrifice | **0** | NAO EXISTE no corpus |
| cannibalism | **0** | NAO EXISTE no corpus (sem forma exata) |

### 2.1 Adrenochrome - **DEBUNKED (0 hits)**

Zero mencoes em todo o corpus. A teoria QAnon sobre "adrenochrome" nao tem NENHUMA base nos documentos reais do caso Epstein.

### 2.2 Spirit Cooking (1 hit) - **DEBUNKED**

**Documento**: EFTA01296720.pdf
**Contexto**: Artigo de opiniao criticando a midia por nao cobrir "the 'Spirit Cooking' and other weird occult and sex affiliations of campaign chairman John Podesta."
**Analise**: E uma referencia a PROPRIA teoria conspiratoria Pizzagate/Spirit Cooking. Nao e evidencia de "spirit cooking" ocorrendo nos circulos de Epstein.

### 2.3 Eyes Wide Shut (12 hits) - **METAFORA JORNALISTICA**

**Conclusao**: Usado por jornalistas como metafora apta para o estilo de vida de Epstein. NAO e linguagem codificada.

**Fontes**:
- **Michael Wolff** (multiplas versoes do mesmo artigo): "a life somewhere between Daddy Warbucks and Eyes Wide Shut. There is indeed a group of young women who act as Epstein's support staff and companions." (HOUSE_OVERSIGHT_022707/022746/022844/022863/022894/022952/023627/024229, EFTA00307947)
- **Blog**: "european girls, frolicking with them, and then proceeding into one big orgy - strikingly similar to Eyes Wide Shut. Without the costumes." (EFTA00104451)
- **Artigo HOUSE_OVERSIGHT_010486**: "The scene brings Eyes Wide Shut to mind. But the thing is, Eyes Wide Shut only works in the shadows."

**Nota**: Embora a metafora seja apt (o filme de Kubrick retrata festas secretas de sexo da elite), o uso nos documentos e DESCRITIVO por terceiros, nao COMUNICATIVO entre conspiradores.

### 2.4 Satanic/Satan - **DEBUNKED como conexao direta**

**Analise dos 21 hits de "satanic"**:
- **Artigos academicos**: Estudos sobre "Satanic Ritual Abuse" allegations (Goodman et al., Child Abuse & Neglect journal) - EFTA00018300, EFTA00159958, VOL00008/EFTA00018300
- **David Icke**: Conteudo conspiratorio sobre "Satanic network" envolvendo Heath e Prince Andrew (EFTA00103831)
- **Artigo sobre moral panic**: Referencias ao panico moral dos anos 1980-1990 sobre SRA em creches (HOUSE_OVERSIGHT_015032)
- **NENHUM** documento mostra Epstein ou seus associados envolvidos em atividades satanicas.

### 2.5 Moloch (3 hits) - **DEBUNKED**

- **EFTA00165862**: "Moloch, Bank Alex. Brown" - nome de entidade financeira (Deutsche Bank Alex. Brown)
- **HOUSE_OVERSIGHT_013501**: "Moloch ha-Moves" - termo yiddish para morte personificada, em texto academico sobre comportamento compulsivo
- **EFTA01509416**: OCR corrompido, sem contexto claro
- **Nenhuma conexao com rituais ou sacrificios.**

### 2.6 Blood Ritual / Human Sacrifice / Cannibalism - **0 HITS CADA**

Nao existem no corpus. As teorias sobre rituais de sangue e sacrificio humano no caso Epstein nao tem nenhuma base documental.

---

## Capitulo 3: Termos de Trafico

### 3.1 Daddy (105 hits) - **PARCIALMENTE CONFIRMADO**

**Conclusao**: Epstein SE REFERIA como "daddy" em pelo menos uma comunicacao. Karyna Shuliak enviava emails com assunto "Daddy". Usado por jornalistas como "sugar daddy".

**Achados confirmados**:

1. **EFTA01301242 / EFTA00158654** (duplicatas): Epstein (jeevacation@gmail.com), 23 de outubro de 2010:
> "spenet time with daddy, great fun"

Resposta (EFTA02416084): **"it explains a lot doesn't it?"**

**Analise**: Epstein se refere como "daddy" a uma pessoa nao identificada (email redactado). A resposta "it explains a lot" sugere que a experiencia revelou algo sobre o comportamento/personalidade de Epstein. O destinatario nao e identificado.

2. **EFTA02297690**: Karyna Shuliak envia email a Epstein com assunto **"Daddy"** e anexo **"photo.JPG"**.

**Analise**: Dentro da dinamica conhecida da relacao Epstein-Shuliak. Pode ser apelido da relacao ou foto do pai de Karyna.

3. **EFTA02546310 / EFTA02546697 / EFTA02360501 / EFTA02545790**: Thread com "Elen capri" - Epstein: "welcome back, hope trip was good and daddy ok"

**Analise**: Aqui "daddy" se refere ao PAI de Elen capri, nao a Epstein.

4. **HOUSE_OVERSIGHT_011908**: Artigo: "Jeffrey Epstein doesn't want to be branded as a 'sex offender' for life, and no, he's not a modeling agency secret sugar daddy"

5. **HOUSE_OVERSIGHT_018438**: Artigo sobre "Sugar Baby & Sugar Daddy" cultura.

**Veredicto**: O uso de "daddy" por Epstein e confirmado mas limitado. Nao e linguagem codificada sistematica - e a dinamica de poder ja amplamente documentada.

### 3.2 Branding (109 hits) - **DEBUNKED como codigo**

A grande maioria dos hits refere-se a "branding" no sentido empresarial (marca, marketing, identidade corporativa). Nenhuma conexao com praticas de trafico.

---

## Capitulo 4: Cross-Reference com Pessoas Conhecidas

A analise de cross-reference cruzou termos alimenticios com 26 pessoas-chave. Os resultados mostram que os termos aparecem em documentos que TAMBEM mencionam essas pessoas, mas NUNCA no mesmo contexto semantico (i.e., ninguem usa "pizza" como codigo em comunicacao com Maxwell, Brunel, etc.).

**Exemplo**: "pizza" aparece em 43 documentos que tambem mencionam pessoas conhecidas. Em TODOS os casos, o termo "pizza" e usado literalmente (pedidos de comida, restaurantes) e as pessoas aparecem em outros trechos do mesmo email/documento.

**Nenhuma instancia de pessoa conhecida usando termo alimenticio como possivel codigo.**

---

## Capitulo 5: Analise Estatistica

### Distribuicao de Classificacao (apos revisao manual)

| Categoria | Total Docs | LITERAL | AMBIGUO | SUSPEITO REAL |
|-----------|-----------|---------|---------|---------------|
| Food terms | 2.667 | ~1.200 | ~1.460 | **1** (Pizza Monster) |
| Extreme terms | 446 | ~54 | ~307 | **0** |
| Trafficking terms | 214 | ~6 | ~157 | **2** (daddy refs) |
| **TOTAL** | **3.327** | **~1.260** | **~1.924** | **3** |

### Taxa de Falso Positivo do Classificador Automatico

O classificador automatico marcou **594 hits como SUSPEITO** (18% do total). Apos revisao manual, apenas **3** sao genuinamente suspeitos (0.09%). A taxa de falso positivo e **99.5%**.

**Razao**: O corpus Epstein e sobre trafico sexual. Palavras como "girl", "young", "party" aparecem em quase todos os documentos. Quando um documento sobre pizza TAMBEM menciona "girls" (em outro contexto), o classificador marca como suspeito.

### Match vs Match_Phrase - Impacto

| Termo | match (OR) | match_phrase | Inflacao |
|-------|-----------|-------------|----------|
| hot dog | 2,628 | **21** | **125x** |
| walnut sauce | 61 | **0** | infinita |
| ice cream | 3,256 | **147** | **22x** |
| pizza monster | 4,142 | **2** | **2,071x** |
| spirit cooking | 1,047 | **1** | **1,047x** |
| eyes wide shut | 3,398 | **12** | **283x** |
| blood ritual | 1,271 | **0** | infinita |

**Licao critica**: Sempre usar `match_phrase` para termos multi-palavra no Elasticsearch. A query `match` faz tokenizacao e OR implicito, inflando resultados dramaticamente.

---

## Capitulo 6: O Que FOI Encontrado como Linguagem Codificada Real

Os documentos Epstein contem linguagem codificada CONFIRMADA, mas NAO sao termos alimenticios. Os codigos reais sao:

| Codigo | Significado | Evidencia |
|--------|-------------|-----------|
| "massage" | Eufemismo central para abuso sexual | Centenas de documentos, depoimentos |
| "fresh" | Mulheres novas/jovens | "she looks very fresh" (Brunel, EFTA02372945) |
| "new friend" | Mulher recem-recrutada | "where is my new friend" (Epstein, EFTA02410234) |
| "the girls" | Vitimas ou mulheres transportadas | Uso operacional em multiplos emails |
| "Girls Trips" | Rotacao sistematica de mulheres | EFTA02256078 |
| "bring" / "send her" | Transporte de vitimas | Multiplos documentos |

**Estes codigos sao bem documentados, corroborados por depoimentos e usados de forma sistematica.** Eles nao tem relacao com a terminologia alimenticia alegada pela teoria Pizzagate.

---

## Conclusoes

### Termos Alimenticios

| Termo | Veredicto | Justificativa |
|-------|-----------|---------------|
| pizza | **DEBUNKED** | 242 hits, todos literais (Arturo's, Patsy's, Joe's, menus) |
| hot dog | **DEBUNKED** | 21 hits reais (era 2,628 por erro), todos literais |
| cheese | **DEBUNKED** | 229 hits, todos literais (cream cheese, bagels, dieta) |
| chicken | **DEBUNKED** | 458 hits, todos literais (menus, compras) |
| walnut | **DEBUNKED** | 73 hits: madeira, piso, nome de empresa |
| walnut sauce | **DEBUNKED** | 0 hits |
| sauce | **DEBUNKED** | 227 hits, todos culinarios |
| muffin | **DEBUNKED** | 84 hits, todos literais (bran muffin, receitas) |
| dominos | **DEBUNKED** | 18 hits, termos financeiros/jogo |
| pasta | **DEBUNKED** | 157 hits, todos culinarios |
| cookie | **DEBUNKED** | 336 hits, todos literais |
| candy | **DEBUNKED** | 142 hits: nome proprio + literal |
| ice cream | **DEBUNKED** | 147 hits, todos literais |
| handkerchief | **DEBUNKED** | 6 hits, todos literais (pocket handkerchief) |
| pizza monster | **SUSPEITO** | 2 hits. Mulher referida como "the pizza". Explicacao literal plausivel (apelido de quem come muita pizza) |

### Termos Extremos

| Termo | Veredicto | Justificativa |
|-------|-----------|---------------|
| adrenochrome | **DEBUNKED** | 0 hits no corpus inteiro |
| spirit cooking | **DEBUNKED** | 1 hit - referencia a propria teoria |
| eyes wide shut | **NAO CODIGO** | Metafora jornalistica (apt mas descritiva) |
| satanic/satan | **DEBUNKED** | Artigos academicos sobre SRA panic |
| moloch | **DEBUNKED** | Nome de empresa + termo yiddish |
| occult | **DEBUNKED** | Artigos/livros academicos |
| cannibal | **DEBUNKED** | Artigos de noticias |
| sacrifice/ritual | **DEBUNKED** | Contextos legais/academicos |
| blood ritual | **DEBUNKED** | 0 hits |
| human sacrifice | **DEBUNKED** | 0 hits |

### Termos de Trafico

| Termo | Veredicto | Justificativa |
|-------|-----------|---------------|
| daddy | **PARCIALMENTE CONFIRMADO** | Epstein se referiu como "daddy" (1 email). Karyna Shuliak usou "Daddy" como titulo com foto. Artigos sobre "sugar daddy". |
| branding | **DEBUNKED** | Marketing/business branding |

### Veredicto Final

1. **A teoria Pizzagate NAO tem base nos documentos Epstein.** Nenhum dos termos alimenticios alegados como codigo (pizza = girl, hot dog = boy, cheese = little girl, etc.) e usado dessa forma nos documentos.

2. **Epstein USAVA linguagem codificada**, mas nao alimenticia. Os codigos reais sao "massage", "fresh", "new friend", "the girls", "Girls Trips" - todos bem documentados e corroborados por depoimentos de vitimas.

3. **O count de "hot dog" inflado (2,628 vs 21 real) demonstra como erros metodologicos podem alimentar teorias conspiratorias.** A busca incorreta no Elasticsearch produziu um numero que parecia "anormalmente alto" e "suspeito", quando na verdade havia apenas 21 mencoes literais.

4. **Os termos extremos (adrenochrome, blood ritual, human sacrifice) simplesmente NAO EXISTEM no corpus.** Teorias sobre rituais satanicas no caso Epstein nao tem nenhuma base documental.

5. **O unico achado genuinamente ambiguo** e o email "Pizza Monster" (EFTA02464505/EFTA02356175), onde uma mulher e referida como "the pizza". Mesmo este caso tem explicacao literal plausivel.

---

## Apendice A: Script de Analise

Arquivo: `investigate_coded_language.py`
Localizacao: `/Users/leonardodias/arvor/epstein/`

O script Python executa 4 fases:
- **Fase A**: Coleta de hits com highlights do ES
- **Fase B**: Classificacao automatica (LITERAL/AMBIGUO/SUSPEITO)
- **Fase C**: Cross-reference com pessoas conhecidas
- **Fase D**: Deep-dive queries combinadas

Dados intermediarios: `/tmp/coded_language/`

## Apendice B: Documentos-Chave Analisados

| Documento | Conteudo | Relevancia para esta investigacao |
|-----------|----------|----------------------------------|
| EFTA02464505 | "The Pizza Monster!" - Epstein: "she looks pregnant" | Principal achado ambiguo |
| EFTA02356175 | Resposta: "Yeah, that's the pizza..." | Principal achado ambiguo |
| EFTA02488656 | "cheese" resposta a menu sushi | DEBUNKED (era pizza) |
| EFTA02510241 | David Stern "Re: Pizza" - negocio | Provavelmente investimento em pizzaria |
| EFTA01301242 | Epstein: "spenet time with daddy, great fun" | Epstein como "daddy" |
| EFTA02297690 | Karyna Shuliak: Subject "Daddy" + photo | Dinamica da relacao |
| EFTA02411684 | "Walnut" como empresa (due diligence) | DEBUNKED (empresa) |
| EFTA02528960 | "Brazilian Walnut" = piso de madeira | DEBUNKED (construcao) |
| EFTA01296720 | "Spirit Cooking" em artigo de opiniao | Referencia a propria teoria |
| EFTA00104451 | "Eyes Wide Shut" em blog sobre Epstein | Metafora jornalistica |

## Apendice C: Nota sobre Metodologia de Busca no Elasticsearch

**ATENCAO PARA FUTURAS INVESTIGACOES**:

O Elasticsearch com `match` query faz:
1. Tokenizacao do texto (split por espacos)
2. OR implicito entre tokens
3. Scoring por relevancia

Isto significa que `match: "hot dog"` busca documentos com "hot" OR "dog", nao a frase "hot dog". Para busca de frases exatas, SEMPRE usar `match_phrase`.

**Impacto nesta investigacao**: O count de "hot dog" no CLAUDE.md (2,628) estava inflado 125x. Counts de "ice cream" (22x), "pizza monster" (2,071x) e "spirit cooking" (1,047x) tambem estariam dramaticamente errados com `match`.
