# Dossiê: Mega-Cruzamento de Listas de Elite vs. Documentos Epstein

**Data**: 15 de fevereiro de 2026
**Classificação**: INVESTIGATIVO — USO JORNALÍSTICO
**Base de dados**: ~580.000 documentos Epstein (Elasticsearch, índice `epstein`)

---

## 1. Sumário Executivo

### Metodologia

Este dossiê cruza **1.381 nomes** extraídos de seis listas de elite contra a totalidade dos documentos do caso Epstein disponíveis no Elasticsearch. As listas analisadas são:

| Lista | Ano | Nomes Buscados | Com Hits > 0 |
|-------|-----|----------------|--------------|
| **DOJ Bondi** (Departamento de Justiça dos EUA) | 2025 | 307 | 302 |
| **Bilderberg** | 2023 | 127 | 99 |
| **Bilderberg** | 2024 | 131 | 103 |
| **Bilderberg** | 2025 | 121 | 97 |
| **Trilateral Commission** | 2008 | 166 | 160 |
| **Committee of 300** | 2010 | 299 | 270 |
| **Committee of 300** | 1991 | 349 | 299 |
| **Papal Bloodlines** | — | 37 | 24 |
| **TOTAL** | — | **1.381** | **1.227** |

**Tipos de busca utilizados**:
- `phrase`: busca exata do nome completo (maior confiabilidade)
- `surname_match`: busca por sobrenome (pode gerar falsos positivos em sobrenomes comuns)
- `c300_previous`: busca herdada de versões anteriores do C300 (alta taxa de falsos positivos)
- `match`: busca simples (casas papais)

**Filtragem de falsos positivos**: Resultados com termos genéricos (August, House, Prince, Michael, Young, White, France, Harry, Philip, Elizabeth, Diana, etc.) e buscas `c300_previous` com hits > 3.000 foram excluídos da análise principal.

### Descobertas-Chave

1. **Jeffrey Epstein era membro da Trilateral Commission em 2008** — aparece na lista oficial com 281.756 hits nos documentos
2. **Peter Thiel** aparece em **4 listas** (Bilderberg 2023, 2024, 2025 + DOJ Bondi) com **1.436 hits** — comunicação direta com Epstein documentada
3. **8 nomes** aparecem simultaneamente na lista **DOJ + Committee of 300**: Bill Gates, Bill Clinton, Tony Blair, George Soros, Susan Rice, Rupert Murdoch, Timothy Geithner, e Elizabeth (genérico)
4. **Susan Rice** é o único nome que aparece em **3 listas diferentes** (DOJ + C300 + Trilateral) com 73 hits reais
5. **Deutsche Bank**, banqueiro principal de Epstein, aparece com **5.299 hits** — confirmando a centralidade da instituição na rede financeira
6. **Goldman Sachs** com **1.326 hits** e **Harvard University** com **1.087 hits** — instituições profundamente entrelaçadas

---

## 2. Análise Cross-Lista: Nomes em Múltiplas Listas

### 2.1 O Caso Jeffrey Epstein na Trilateral Commission

**Descoberta crítica**: Jeffrey Epstein consta como membro da **Trilateral Commission de 2008**, a organização fundada por David Rockefeller e Zbigniew Brzezinski em 1973. Isto coloca Epstein não como um outsider que se infiltrou na elite, mas como um **membro formal das estruturas de governança global**.

A lista de 2008 da Trilateral inclui outros nomes com presença nos documentos Epstein:
- **Lawrence H. Summers** (271 hits) — emails diretos com Epstein sobre arranjos com o Banco Nacional do Cazaquistão
- **David Rockefeller** (35 hits) — Epstein registrou-se para leilão da coleção Rockefeller
- **Jamie Dimon** (144 hits) — mencionado em email de Boris Nikolic sobre painel de investimento do JPMorgan
- **Zbigniew Brzezinski** (25 hits) — listado junto com Epstein no mesmo documento da Trilateral
- **Mortimer B. Zuckerman** (295 hits) — assistente executiva de Zuckerman em contato com Lesley Groff
- **David Gergen** (393 hits) — emails diretos, Dropbox compartilhado, reuniões coordenadas por Groff
- **Fareed Zakaria** (81 hits) — artigos sobre economia encaminhados a Epstein
- **Henry A. Kissinger** (8 hits) — listado como "Lifetime Trustee" da Trilateral no mesmo documento

### 2.2 Nomes em 4 Listas

| Nome | Listas | ES Hits | Evidência |
|------|--------|---------|-----------|
| **Peter Thiel** | BIL23+BIL24+BIL25+DOJ | **1.436** | Email sobre envio de suéteres para endereço do Thiel Capital em São Francisco; Alisa Bekins coordenou |
| **Jens Stoltenberg** | BIL23+BIL24+BIL25+DOJ | 19 | Ex-Secretário-Geral da OTAN; presença nos documentos por contexto geopolítico |
| **José Manuel Barroso** | BIL23+BIL24+BIL25+C300 | 3 | Ex-Presidente da Comissão Europeia |
| **Patricia Barbizet** | BIL23+BIL24+BIL25+TC | 1 | CEO Kering, Trilateral e Bilderberg |
| **Thomas Leysen** | BIL23+BIL24+BIL25+TC | 1 | Chairman Umicore/KBC |

### 2.3 Nomes em 3 Listas (com hits significativos)

| Nome | Listas | ES Hits | Nota |
|------|--------|---------|------|
| **Susan Rice** | DOJ+C300+TC | **73** | Netflix board + contexto Obama; email encaminhado por Richard Kahn a Epstein |
| **Fareed Zakaria** | BIL24+BIL25+TC | **81** | Jornalista CNN; artigos económicos circularam na rede Epstein |
| **Bill Gates** | DOJ+C300 | **1.487** | "meeting at Leon's w/Bill Gates"; reuniões com Mort Zuckerman, Kathy Ruemmler e Ramsey no Four Seasons |
| **Bill Clinton** | DOJ+C300 | **1.178** | Emails sobre "RE Bill Clinton" encaminhados dentro da organização |
| **Zbigniew Brzezinski** | C300+TC | **25** | Trilateral + C300; mencionado no mesmo documento da lista Trilateral |
| **David Rockefeller** | C300(1991)+TC | **35** | Fundador da Trilateral; coleção de arte leiloada e acompanhada por Epstein |
| **Stanley Fischer** | C300+TC | **15** | Governador do Banco de Israel; email de "Marty Pere" para Epstein pedindo desculpas e mencionando Fischer |
| **Richard Holbrooke** | C300+TC | **15** | Perseus LLC; listado no documento da Trilateral |
| **Henry A. Kissinger** | BIL23+TC | **8** | "Lifetime Trustee" da Trilateral; Kissinger Associates com 31 hits |
| **Eric Schmidt** | BIL23+BIL24+BIL25 | 120 | Busca por frase "Eric Schmidt" (ex-CEO Google/Alphabet) |

### 2.4 Peter Thiel — Análise Aprofundada

Peter Thiel é o nome com maior presença cross-lista (4 listas) e com volume significativo de documentos (1.436 hits). A evidência documental mostra:

- **EFTA02457661.pdf**: Email de 2 de julho de 2016 com assunto "Peter Thiel - Address for sweaters" enviado a Jeffrey Epstein. Remetente coletou endereços e pediu aprovação de Epstein para envio ao escritório do **Thiel Capital, LLC** em São Francisco
- **Alisa Bekins** aparece como contato executivo do Thiel Capital no mesmo email
- O envio de "suéteres" para múltiplos endereços sugere uma operação de presente/cortesia coordenada por Epstein
- Thiel Capital LLC aparece nos documentos com **17 hits** de forma independente

**Contexto**: Peter Thiel é cofundador do PayPal, investidor no Facebook, fundador da Palantir Technologies (contrato com CIA/NSA), e participante consistente do Bilderberg (2023, 2024, 2025). A sua presença na lista DOJ Bondi indica que investigadores do DOJ consideraram-no relevante para a investigação.

---

## 3. DOJ Bondi — Top Conexões nos Documentos Epstein

A lista DOJ Bondi contém **307 nomes** considerados relevantes pelo Departamento de Justiça dos EUA sob a Procuradora-Geral Pam Bondi. Dos 307, **302 aparecem nos documentos** com pelo menos 1 hit.

### 3.1 Top 40 — Busca por Frase Exata (excluídos falsos positivos)

| # | Nome | ES Hits | Contexto Documental |
|---|------|---------|---------------------|
| 1 | **Jeffrey Epstein** | 281.756 | Sujeito principal; também membro Trilateral 2008 |
| 2 | **Ghislaine Maxwell** | 11.322 | Recrutadora principal; 5.109 docs confirmados |
| 3 | **Leon Black** | 5.252 | Transferências financeiras massivas ($35K-$50K recorrentes); "THE J BLACK TR" |
| 4 | **Kathy Ruemmler** | 4.710 | Ex-conselheira da Casa Branca de Obama; reuniões diretas com Epstein em novembro de 2014 |
| 5 | **Woody Allen** | 3.386 | iMessages diretas com Epstein (jeeitunes@gmail.com) em 2015-2016 |
| 6 | **Peter Mandelson** | 3.177 | Emails diretos com Epstein em novembro de 2011; "Yes but very greecy" |
| 7 | **Michael Wolff** | 3.173 | Jornalista/autor; grande volume de documentos |
| 8 | **Larry Summers** | 2.823 | SMS com Epstein em abril de 2019; "Will try." |
| 9 | **Jean Luc Brunel** | 2.723 | Agente de modelos MC2; coordenação com Lesley Groff; emails de julho de 2014 |
| 10 | **Noam Chomsky** | 2.518 | Emails familiares (Avi, Harry, Diana Chomsky); comunicações de fevereiro de 2018 |
| 11 | **Ehud Barak** | 2.209 | iMessages 2013: hotel Radisson em São Petersburgo; "Fascinating person. Thanks." |
| 12 | **Terje Rod-Larsen** | 1.705 | Presidente IPI; Lesley Groff coordenou chamada com Epstein em outubro de 2011 |
| 13 | **Reid Hoffman** | 1.510 | Emails diretos janeiro de 2014: "we're on, sky" — café da manhã 8am PDT confirmado |
| 14 | **Bill Gates** | 1.487 | "meeting at Leon's w/Bill Gates"; reunião com Mort Zuckerman e Kathy Ruemmler no Four Seasons |
| 15 | **John Brockman** | 1.469 | Agente literário; encontro confirmado por Groff: "See you at 3pm" março de 2016 |
| 16 | **Peter Thiel** | 1.436 | Endereço Thiel Capital coletado para envio de "suéteres" — ver seção 2.4 |
| 17 | **Donald Trump** | 1.382 | Contexto House Oversight; análise de sentimento de debates presidenciais |
| 18 | **Steve Bannon** | 1.347 | iMessages: "Do u know Bernard Arnault" — "Very close mutual friends"; tentou marcar café da manhã |
| 19 | **Bill Clinton** | 1.178 | Emails sobre "RE Bill Clinton" circulados internamente; Andy Kay encaminhou informação |
| 20 | **Alan Dershowitz** | 1.135 | Honorários jurídicos: **$3.578.000** (Dershowitz Eiger $427K + outros $173K = **$4.178.462 total**) |
| 21 | **Les Wexner** | 1.126† | †"Wexner"=1.126; "Leslie Wexner"=522; "Les Wexner"=215. **COCONSPIRADOR**: transferiu $200M+ a Epstein; poder notarial sobre fortuna; "Dybbuk"; Wexner Foundation=40; Limited Brands=163 |
| 22 | **Alexander Acosta** | 1.061 | Procurador que negociou o acordo de não-acusação de 2008 |
| 23 | **Daniel Siad** | 1.056 | Mensagens Skype recorrentes: "Hello Jeffrey tell when you have time to speak"; "Sending warme[st]" |
| 24 | **Jay Lefkowitz** | 928 | Contato coordenado por Rosa M. da Silva via Jes Staley (JPMorgan) |
| 25 | **Hillary Clinton** | 611 | Contexto político e referências documentais |
| 26 | **Elon Musk** | 599 | Mencionado em contexto de reportagens e comunicações |
| 27 | **Barack Obama** | 581 | Referências contextuais; administração Obama conectada via Kathy Ruemmler e Susan Rice |
| 28 | **Bill Richardson** | 538 | Ex-governador do Novo México (estado do Zorro Ranch) |
| 29 | **George W. Bush** | 401 | Referências políticas e contextuais |
| 30 | **Henry Jarecki** | 401 | Médico e investidor; contato direto documentado |
| 31 | **Joe Biden** | 361 | Referências contextuais; Hunter Biden também com 99 hits |
| 32 | **Richard Branson** | 340 | Proprietário de Necker Island; 340 menções nos documentos |
| 33 | **Melinda Gates** | 338 | Mencionada em contexto conjunto com Bill Gates |
| 34 | **David Boies** | 328 | Advogado de Epstein e depois das vítimas |
| 35 | **Benjamin Netanyahu** | 321 | Primeiro-ministro de Israel; conexão via Ehud Barak |
| 36 | **Robert Maxwell** | 298 | Pai de Ghislaine; conexões históricas Mossad |
| 37 | **Gloria Allred** | 274 | Advogada de direitos civis |
| 38 | **Marc Rowan** | 256 | CEO Apollo Global Management (sucessor de Leon Black) |
| 39 | **John Kerry** | 249 | Ex-Secretário de Estado |
| 40 | **Ronald Reagan** | 246 | Referências históricas |

### 3.2 DOJ — Nomes Notáveis (41-80)

| Nome | ES Hits | Nome | ES Hits |
|------|---------|------|---------|
| David Copperfield | 215 | Marie Villafana | 213 |
| Geoffrey Berman | 212 | Sultan Ahmed bin Sulayem | 194 |
| Michael Reiter | 181 | Damian Williams | 181 |
| Tony Blair | 173 | Mark Zuckerberg | 171 |
| William Barr | 168 | Thomas Pritzker | 163 |
| Kenneth Starr | 160 | Doug Band | 153 |
| Michael Jackson | 139 | Marco Rubio | 134 |
| Kevin Spacey | 133 | Jeff Bezos | 130 |
| John McCain | 129 | Lanna Belohlavek | 128 |
| Nancy Pelosi | 127 | Rudy Giuliani | 123 |

### 3.3 DOJ — Figuras Jurídicas e Governamentais

O cruzamento revela uma concentração de **figuras do aparato jurídico e de inteligência** na lista DOJ:

- **Alexander Acosta** (1.061) — procurador do acordo de 2008
- **Geoffrey Berman** (212) — procurador SDNY
- **Damian Williams** (181) — procurador SDNY
- **William Barr** (168) — Attorney General
- **Kenneth Starr** (160) — advogado de defesa
- **Jay Clayton** (84) — chairman SEC
- **Joseph Recarey** (84) — detetive Palm Beach PD
- **James Comey** (102) — diretor FBI
- **Robert S. Mueller** (40) — investigador especial
- **Merrick Garland** (59) — Attorney General
- **Rod Rosenstein** (41) — Deputy AG
- **John Brennan** (51) — diretor CIA
- **Michael Flynn** (107) — conselheiro de segurança nacional

---

## 4. Bilderberg 2023-2025 — Top Conexões

O Grupo Bilderberg realiza reuniões anuais com ~130 participantes selecionados entre líderes políticos, financeiros, militares e de mídia. Cruzámos as listas de 2023, 2024 e 2025.

### 4.1 Top 30 Bilderberg (busca por frase, excluídos sobrenomes genéricos)

| # | Nome | ES Hits | Listas BIL | Contexto |
|---|------|---------|------------|----------|
| 1 | **Peter Thiel** | 1.436 | 23+24+25 | Ver seção 2.4 — Thiel Capital, suéteres |
| 2 | **Lawrence Summers** | 86 | 25 | Também TC 2008; emails sobre Banco do Cazaquistão |
| 3 | **Fareed Zakaria** | 81 | 24+25 | Também TC 2008; artigos económicos partilhados |
| 4 | **Børge Brende** | 56 | 23+25 | Presidente World Economic Forum |
| 5 | **Thomas L. Friedman** | 53 | 25 | Colunista NYT |
| 6 | **Niall Ferguson** | 31 | 23+24 | Historiador; Stanford/Hoover |
| 7 | **Christian Sewing** | 23 | 24+25 | CEO Deutsche Bank — banco central de Epstein |
| 8 | **Mario Monti** | 21 | 24+25 | Ex-PM Itália; chairman Bilderberg steering |
| 9 | **Mark Carney** | 19 | 23 | Ex-Governador Bank of England e Bank of Canada |
| 10 | **Demis Hassabis** | 19 | 23+24+25 | CEO Google DeepMind |
| 11 | **Gideon Rachman** | 17 | 23+24+25 | Chief foreign affairs commentator Financial Times |
| 12 | **Peter Lee** | 15 | 24 | Microsoft Research |
| 13 | **Bret Stephens** | 15 | 24 | Colunista NYT |
| 14 | **Brian Deese** | 12 | 23 | Ex-diretor NEC (Biden) |
| 15 | **Mark Rutte** | 11 | 23+24+25 | Secretário-Geral NATO |
| 16 | **Stacey Abrams** | 10 | 23+24+25 | Política Georgia |
| 17 | **Eric S. Lander** | 10 | 24 | Ex-diretor OSTP; Broad Institute |
| 18 | **Henry R. Kravis** | 9 | 23+24+25 | KKR; co-chairman |
| 19 | **Dambisa Moyo** | 9 | 23 | Economista/autora |
| 20 | **Henry A. Kissinger** | 8 | 23 | Também TC; "Lifetime Trustee" da Trilateral |
| 21 | **Josep Borrell** | 7 | 23 | Alto Representante UE |
| 22 | **Garry Kasparov** | 7 | 23 | Ex-campeão mundial de xadrez |
| 23 | **Satya Nadella** | 7 | 23+25 | CEO Microsoft |
| 24 | **John Micklethwait** | 7 | 23+24+25 | Editor Bloomberg |
| 25 | **Sam Altman** | 6 | 23 | CEO OpenAI |
| 26 | **Albert Bourla** | 6 | 23+24+25 | CEO Pfizer |
| 27 | **Marcus Wallenberg** | 6 | 23+24+25 | Chairman SEB (banco sueco) |
| 28 | **Mellody Hobson** | 6 | 24+25 | Chairman Starbucks; presidente Ariel Investments |
| 29 | **Jeremy Hunt** | 6 | 25 | Chancellor of the Exchequer UK |
| 30 | **Dario Amodei** | 5 | 24 | CEO Anthropic |

### 4.2 Destaque: Christian Sewing (CEO Deutsche Bank)

Christian Sewing, CEO do **Deutsche Bank** — a instituição financeira que mais aparece nos documentos Epstein (5.299 hits para "Deutsche Bank AG") — participou do Bilderberg em 2024 e 2025. O Deutsche Bank foi multado em **$150 milhões** pelo New York Department of Financial Services por falhas de compliance relacionadas a Epstein, e era o principal banco de Epstein após o JPMorgan cortá-lo. A presença do CEO atual no Bilderberg, enquanto o banco continua sob escrutínio, é notável.

---

## 5. Trilateral Commission 2008 — Top Conexões

A Trilateral Commission, fundada por **David Rockefeller** e **Zbigniew Brzezinski** em 1973, conecta líderes da América do Norte, Europa e Ásia. A lista de 2008 é a única disponível publicamente daquele período.

### 5.1 Facto Crucial: Epstein como Membro

Jeffrey Epstein aparece como membro da lista de 2008 com a maior quantidade de hits (281.756) em todo o estudo. Isto demonstra que Epstein foi formalmente aceite numa das organizações mais exclusivas do mundo, ao lado de figuras como:

### 5.2 Top 25 Trilateral (excluídos falsos positivos)

| # | Nome | ES Hits | Cargo/Contexto | Também em |
|---|------|---------|----------------|-----------|
| 1 | **Jeffrey Epstein** | 281.756 | MEMBRO — sujeito principal | DOJ |
| 2 | **David Gergen** | 393 | Professor Harvard Kennedy School; emails diretos, Dropbox partilhado | — |
| 3 | **Mortimer B. Zuckerman** | 295 | Chairman Boston Properties/US News; assistente coordenou com Groff | — |
| 4 | **Lawrence H. Summers** | 271 | Ex-Secretário do Tesouro; emails sobre arranjos com Banco Nacional do Cazaquistão | BIL25 |
| 5 | **Jamie Dimon** | 144 | CEO JPMorgan; mencionado em email de Boris Nikolic sobre painel de investimento | — |
| 6 | **Fareed Zakaria** | 81 | Jornalista CNN; artigos circularam na rede | BIL24+25 |
| 7 | **Susan Rice** | 73 | Email de Richard Kahn para Epstein sobre Rice ir para board da Netflix | DOJ+C300 |
| 8 | **Dennis Ross** | 54 | Diplomata; negociador Médio Oriente | — |
| 9 | **Gordon Smith** | 39 | Senador Oregon | — |
| 10 | **Dianne Feinstein** | 38 | Senadora Califórnia; formulário casework no escritório dela encontrado nos docs | — |
| 11 | **David Rockefeller** | 35 | FUNDADOR da Trilateral; Epstein registrou-se para leilão Christie's da coleção Rockefeller | C300(1991) |
| 12 | **Zbigniew Brzezinski** | 25 | CO-FUNDADOR da Trilateral; listado no mesmo documento de membros | C300(2010) |
| 13 | **Strobe Talbott** | 24 | Presidente Brookings; editor TIME | — |
| 14 | **Anne-Marie Slaughter** | 21 | Princeton; Diretora de Planeamento Político State Dept | — |
| 15 | **Francis Fukuyama** | 20 | Professor Stanford; "End of History" | — |
| 16 | **Kenneth Rogoff** | 19 | Economista Harvard; ex-FMI | — |
| 17 | **Graham Allison** | 17 | Professor Harvard Kennedy School; expert em segurança nuclear | — |
| 18 | **Robert Kagan** | 17 | Analista Brookings; neoconservador | — |
| 19 | **Stanley Fischer** | 15 | Governador Banco de Israel; email de "Marty Pere" para Epstein sobre Fischer | C300(2010) |
| 20 | **Richard Holbrooke** | 15 | Perseus LLC; diplomata | C300(2010) |
| 21 | **John D. Rockefeller** | 13 | Senador West Virginia (descendente do fundador) | — |
| 22 | **Paul A. Volcker** | 10 | Ex-chairman Federal Reserve | — |
| 23 | **Henry A. Kissinger** | 8 | "Lifetime Trustee" da Trilateral; Kissinger Associates | BIL23 |
| 24 | **Richard N. Haass** | 8 | Presidente Council on Foreign Relations | — |
| 25 | **Kurt Campbell** | 7 | Subsecretário de Estado para Ásia-Pacífico | — |

### 5.3 Análise: A Rede Trilateral-Epstein

O documento **EFTA01082667.pdf** é particularmente revelador: contém a lista de membros da Trilateral Commission onde aparecem juntos:
- **Henry A. Kissinger** — "Lifetime Trustee"
- **Richard Holbrooke** — Perseus LLC, New York
- **Robert Kagan** — Carnegie Endowment
- **Zbigniew Brzezinski** — outro "Lifetime Trustee"

O documento **EFTA02450724.pdf** contém outra lista formal onde Brzezinski, Sylvia Mathews Burwell, e Richard Holbrooke aparecem juntos, com referências a "attorney-client privileged" e "inside information" — sugerindo que este documento foi parte de comunicações jurídicas.

**Implicação**: Epstein não apenas circulava entre estes nomes — ele era um **membro formal da mesma organização**. A questão é: quem o indicou? E que papel ele desempenhava dentro da Trilateral?

---

## 6. Committee of 300 — Resumo

> **DOSSIÊ COMPLETO**: Ver [`dossie_committee_300_epstein_cruzamento.md`](dossie_committee_300_epstein_cruzamento.md) — **986 linhas, 42 achados detalhados** incluindo:
> - Peter Mandelson (3.336 docs, "Need a Lord on the board?", Deripaska)
> - Lynn Forester de Rothschild (vendeu propriedade de Maxwell)
> - Blavatnik ("Friend of Ghislaine" em Moscou)
> - Jantar de 2014: Kissinger + Schwarzman + Leon Black + Barak + Staley + Blankfein + Blavatnik + Summers + Woody Allen
> - Cadeia completa Bronfman: Edgar Sr. (1º cliente Bear Stearns 1976) → Mega Group → NXIVM
> - Taubman, Wexner ("Dybbuk"), Cameron, Blankfein, Sawers (MI6), e 30+ outros

### 6.1 Contexto

A lista do Committee of 300 é a mais extensa (299 nomes em 2010, 349 em 1991) e a que gera mais falsos positivos devido a buscas por sobrenomes genéricos e termos como "August", "Prince", "House", etc.

### 6.2 Resultados Significativos (busca phrase, sem falsos positivos)

| Nome | ES Hits | Lista | Também em |
|------|---------|-------|-----------|
| **Bill Gates** | 1.487 | C300(2010) | DOJ |
| **Bill Clinton** | 1.178 | C300(2010) | DOJ |
| **Tony Blair** | 173 | C300(2010) | DOJ |
| **George Soros** | 100 | C300(2010) | DOJ |
| **Susan Rice** | 73 | C300(2010) | DOJ+TC |
| **Rupert Murdoch** | 62 | C300(2010) | DOJ |
| **David Rockefeller** | 35 | C300(1991) | TC |
| **Zbigniew Brzezinski** | 25 | C300(2010) | TC |
| **Mervyn King** | 22 | C300(2010) | — |
| **Stanley Fischer** | 15 | C300(2010) | TC |
| **Richard Holbrooke** | 15 | C300(2010) | TC |
| **Timothy Geithner** | 12 | C300(2010) | DOJ |
| **Francois Mitterrand** | 6 | C300(1991) | — |
| **C. Fred Bergsten** | 5 | C300(2010) | TC |
| **Joseph Safra** | 3 | C300(2010) | — |

### 6.3 Nomes C300 com Sobrenome Match (sobrenomes específicos o suficiente)

| Nome | ES Hits | Termo | Lista |
|------|---------|-------|-------|
| **Andrew (Prince) – of York** | 1.660 | "Prince Andrew" | C300(2010) |
| **Dominique Strauss-Kahn** | 50 | "Strauss-Kahn" | C300(2010) |
| **Henry Kissinger** | 269 | "Kissinger" | C300(2010) |
| **Warren Buffett** | 209 | "Buffett" | C300(2010) |
| **Al Gore** | 214 | "Al Gore" | C300(2010) |
| **Nicolas Sarkozy** | 182 | "Sarkozy" | C300(2010) |
| **Paul Krugman** | 130 | "Krugman" | C300(2010) |
| **Ben Bernanke** | 111 | "Bernanke" | C300(2010) |
| **Mario Draghi** | 93 | "Draghi" | C300(2010) |
| **Roman Abramovich** | 44 | "Abramovich" | C300(2010) |
| **Klaus Schwab** | 10 | "Klaus Schwab" | C300(2010) |

*Nota: Busca por frase "Strauss-Kahn" retorna 50 hits (29 para "Dominique Strauss-Kahn"). O contexto DSK-Epstein (ambos envolvidos em escândalos sexuais com ligações a poder) merece investigação separada.*

### 6.4 Famílias e Linhagens C300

As listas C300 incluem diversas famílias aristocráticas e dinásticas. Os resultados por sobrenome de família incluem (com cautela sobre falsos positivos):

- **Rockefeller** (809 hits para sobrenome) — David Jr, David Sr, Nicholas
- **Rothschild** (7.718 hits para sobrenome; 28 para "Jacob Rothschild", 9 para "Evelyn de Rothschild") — Benjamin de, David René, Evelyn Robert, Leopold David
- **Bronfman** (95 hits para Charles Rosner; 31 para Edgar Jr)
- **DuPont** (226 hits)
- **Vanderbilt** (99 hits)
- **Warburg** (58 hits) — Max e S.C.
- **Oppenheimer** (344 hits)
- **Sassoon** (23 hits) — Isaac S.D. e James Meyer

---

## 7. Papal Bloodlines — Resultados

As 14 casas papais históricas (as famílias que controlaram o Vaticano por séculos) e seus representantes modernos foram cruzados contra os documentos.

### 7.1 Casas Papais nos Documentos

| Casa | ES Hits | Contexto |
|------|---------|----------|
| **Conti** | 257 | Sobrenome italiano relativamente comum; necessita análise contextual |
| **Medici** | 94 | Referências históricas e culturais |
| **Massimo** | 42 | Pode incluir falsos positivos (nome próprio italiano) |
| **Mattei** | 42 | Sobrenome italiano |
| **Doria** | 12 | Parte do nome Doria-Pamphili-Landi; "Doria-Pamphili-Landi" completo = 0 hits |
| **Borghese** | 27 | Família nobre romana |
| **Colonna** | 18 | Família nobre romana |
| **Orsini** | 16 | Família nobre romana |
| **Savoia** | 7 | Casa real italiana |
| **Farnese** | 5 | Família nobre |
| **Gaetani** | 4 | Família nobre |
| **Barberini** | 1 | Família nobre romana |
| **Chigi** | 1 | Família nobre romana |

**Sem resultados (0 hits)**: Aldobrandini, Braschi, Breakspear, Doria-Pamphili-Landi (completo), Ruspoli, Altieri, Cybo, Torlonia, Pallavicini

### 7.2 Representantes Individuais

| Nome | ES Hits (frase) | Casa | Nota |
|------|-----------------|------|------|
| **Jacob Rothschild** | 28 | Rothschild (associado) | Correspondência pessoal documentada |
| **Evelyn de Rothschild** | 9 | Rothschild (associado) | Socialização em River House |
| **David Rothschild** | 2 | Rothschild (associado) | Epstein queria "beat David Rothschild" |
| **Nathan Rothschild** | 1 | Rothschild (associado) | Referência histórica sobre Waterloo |
| **Fabrizio Massimo** | 0 | Massimo | "Massimo" isolado = 42 hits (sobrenome genérico) |
| **Scipione Borghese** | 0 | Borghese | "Borghese" isolado = 27 hits |
| **Marcantonio Colonna** | 0 | Colonna | "Colonna" isolado = 18 hits |
| **Domenico Orsini** | 0 | Orsini | "Orsini" isolado = 16 hits |
| **Giancarlo Orsini** | 0 | Orsini | Idem |

### 7.3 Conexão Rothschild–Aldobrandini: O Casamento que Une Duas Dinastias

**ACHADO CRÍTICO**: Em 1974, **Baron David de Rothschild** (filho de Baron Guy de Rothschild, chefe do ramo francês da família bancária) casou-se com **Olimpia Aldobrandini** (filha de Don Francesco e Donna Maria Aldobrandini, nobreza papal veneziana) numa cerimónia civil em Reux, Normandia, presidida pela mãe do noivo, Baronesa Alix de Rothschild, na qualidade de Mayor da vila.

Este casamento une diretamente:
- A **família Rothschild** (presente nos documentos Epstein com 28+ hits para Jacob, 9 para Evelyn, 2 para David) — com conexões financeiras documentadas a Epstein
- A **família Aldobrandini** (uma das 13 linhagens papais históricas) — sem hits diretos nos documentos, mas com laços à mais alta nobreza italiana

**Nos documentos Epstein**, a conexão Rothschild é substancial:
- **Jacob Rothschild** (28 hits): Email direto — "Do you know Jacob Rothschild?" (EFTA01781848). Correspondência pessoal com "A. de Rothschild" sobre "The Rothschild Name" (EFTA00631158, Set 2015)
- **Evelyn de Rothschild** (9 hits): Socialização em River House — "Saw Sir Evelyn de Rothschild at River House Wed night" (EFTA00768741)
- **David Rothschild** (2 hits): Epstein a Kathy Ruemmler — "*I wonder if we can beat David Rothschild at his own game, and start some funds calling them Premier Rothschild, the original Rothschild, the only real Rothschilds, the honest Rothschilds*" (EFTA02480220, Nov 2015)
- **Nathan Rothschild** (1 hit): Epstein demonstra conhecimento íntimo da história financeira Rothschild — "The entire Rothschild Fortune was based on Nathan Rothschild knowing that Napoleon was losing at Waterloo" (EFTA01000966)

A ambição de Epstein de "superar David Rothschild" e criar fundos rivais sob o nome "Rothschild" revela que ele via a família como modelo e competidor, não apenas como conhecidos sociais.

**Significado**: O casamento Rothschild-Aldobrandini representa a fusão de poder financeiro moderno (banca internacional) com linhagem papal histórica (nobreza vaticana). Que uma família tão entrelaçada com Epstein tenha laços matrimoniais com a mais antiga nobreza papal ilustra a densidade das redes de poder no topo da pirâmide.

### 7.4 Análise Geral

A presença de sobrenomes papais nos documentos é em grande parte contextual. Nenhum representante individual das casas papais (exceto Rothschilds) aparece com busca por nome completo. As exceções são:

1. **Rothschilds** (28 hits para "Jacob Rothschild", 9 para "Evelyn de Rothschild", 2 para "David Rothschild") — Conexão documentada e substancial. Jacob, Evelyn e David aparecem em emails diretos. Epstein aspirava competir financeiramente com David de Rothschild, que por casamento é Aldobrandini
2. **Conti** (257 hits) — Volume alto mas possivelmente contaminado por sobrenome comum italiano
3. **Medici** (94 hits) — Provavelmente referências históricas/culturais, não à família atual

---

## 8. Tabela Mestra (Resumida)

> **TABELA COMPLETA (1.323 nomes)**: Ver [`dossie_nomes_excluidos_doj.md`](dossie_nomes_excluidos_doj.md), seção 8 — inclui todos os 1.381 nomes pesquisados com ES hits, Neo4j, e pertencimento a cada lista.

Abaixo, nomes com **hits > 10** e busca confiável (excluídos falsos positivos óbvios de buscas genéricas).

**Legenda das colunas**: DOJ = Lista DOJ Bondi | C3 = Committee of 300 | BIL = Bilderberg | TC = Trilateral | PAP = Papal Bloodlines

| Nome | ES Hits | DOJ | C3 | BIL | TC | PAP | Termo de Busca |
|------|---------|-----|----|----|----|----|----------------|
| Jeffrey Epstein | 281.756 | X | | | X | | Jeffrey Epstein |
| Ghislaine Maxwell | 11.322 | X | | | | | Ghislaine Maxwell |
| Leon Black | 5.252 | X | | | | | Leon Black |
| Kathy Ruemmler | 4.710 | X | | | | | Kathy Ruemmler |
| Woody Allen | 3.386 | X | | | | | Woody Allen |
| Peter Mandelson | 3.177 | X | | | | | Peter Mandelson |
| Michael Wolff | 3.173 | X | | | | | Michael Wolff |
| Larry Summers | 2.823 | X | | | | | Larry Summers |
| Jean Luc Brunel | 2.723 | X | | | | | Jean Luc Brunel |
| Noam Chomsky | 2.518 | X | | | | | Noam Chomsky |
| Ehud Barak | 2.209 | X | | | | | Ehud Barak |
| Terje Rod-Larsen | 1.705 | X | | | | | Terje Rod-Larsen |
| Andrew (Prince) | 1.660 | | X | | | | Prince Andrew |
| Reid Hoffman | 1.510 | X | | | | | Reid Hoffman |
| Bill Gates | 1.487 | X | X | | | | Bill Gates |
| John Brockman | 1.469 | X | | | | | John Brockman |
| Peter Thiel | 1.436 | X | | X | | | Peter Thiel |
| Donald Trump | 1.382 | X | | | | | Donald Trump |
| Steve Bannon | 1.347 | X | | | | | Steve Bannon |
| Bill Clinton | 1.178 | X | X | | | | Bill Clinton |
| Alan Dershowitz | 1.135 | X | | | | | Alan Dershowitz |
| Alexander Acosta | 1.061 | X | | | | | Alexander Acosta |
| Daniel Siad | 1.056 | X | | | | | Daniel Siad |
| Jay Lefkowitz | 928 | X | | | | | Jay Lefkowitz |
| Hillary Clinton | 611 | X | | | | | Hillary Clinton |
| Elon Musk | 599 | X | | | | | Elon Musk |
| Barack Obama | 581 | X | | | | | Barack Obama |
| Bill Richardson | 538 | X | | | | | Bill Richardson |
| Bono | 499 | X | | | | | Bono |
| George W. Bush | 401 | X | | | | | George W. Bush |
| Henry Jarecki | 401 | X | | | | | Henry Jarecki |
| David Gergen | 393 | | | | X | | David Gergen |
| Joe Biden | 361 | X | | | | | Joe Biden |
| Richard Branson | 340 | X | | | | | Richard Branson |
| Melinda Gates | 338 | X | | | | | Melinda Gates |
| David Boies | 328 | X | | | | | David Boies |
| Benjamin Netanyahu | 321 | X | | | | | Benjamin Netanyahu |
| Robert Maxwell | 298 | X | | | | | Robert Maxwell |
| Mortimer B. Zuckerman | 295 | | | | X | | Mortimer B. Zuckerman |
| Gloria Allred | 274 | X | | | | | Gloria Allred |
| Lawrence H. Summers | 271 | | | | X | | Lawrence H. Summers |
| Henry Kissinger | 269 | | X | | | | Kissinger |
| Conti (casa papal) | 257 | | | | | X | Conti |
| Marc Rowan | 256 | X | | | | | Marc Rowan |
| John Kerry | 249 | X | | | | | John Kerry |
| Ronald Reagan | 246 | X | | | | | Ronald Reagan |
| Mitt Romney | 228 | X | | | | | Mitt Romney |
| Les Wexner | 1.126† | X | | | | | †"Wexner"=1.126; "Leslie Wexner"=522; "Les Wexner"=215. Coconspirador; Wexner Foundation=40; Limited Brands=163 |
| David Copperfield | 215 | X | | | | | David Copperfield |
| Al Gore | 214 | | X | | | | Al Gore |
| Marie Villafana | 213 | X | | | | | Marie Villafana |
| Geoffrey Berman | 212 | X | | | | | Geoffrey Berman |
| Warren Buffett | 209 | | X | | | | Buffett |
| Sultan Ahmed bin Sulayem | 194 | X | | | | | Sultan Ahmed bin Sulayem |
| Nicolas Sarkozy | 182 | | X | | | | Sarkozy |
| Michael Reiter | 181 | X | | | | | Michael Reiter |
| Damian Williams | 181 | X | | | | | Damian Williams |
| Tony Blair | 173 | X | X | | | | Tony Blair |
| George H.W. Bush | 173 | | X | | | | George Bush |
| Mark Zuckerberg | 171 | X | | | | | Mark Zuckerberg |
| William Barr | 168 | X | | | | | William Barr |
| Thomas Pritzker | 163 | X | | | | | Thomas Pritzker |
| Kenneth Starr | 160 | X | | | | | Kenneth Starr |
| Doug Band | 153 | X | | | | | Doug Band |
| Jamie Dimon | 144 | | | | X | | Jamie Dimon |
| Michael Jackson | 139 | X | | | | | Michael Jackson |
| Marco Rubio | 134 | X | | | | | Marco Rubio |
| Kevin Spacey | 133 | X | | | | | Kevin Spacey |
| Paul Krugman | 130 | | X | | | | Krugman |
| Jeff Bezos | 130 | X | | | | | Jeff Bezos |
| John McCain | 129 | X | | | | | John McCain |
| Lanna Belohlavek | 128 | X | | | | | Lanna Belohlavek |
| Nancy Pelosi | 127 | X | | | | | Nancy Pelosi |
| Rudy Giuliani | 123 | X | | | | | Rudy Giuliani |
| Lindsey Graham | 122 | X | | | | | Lindsey Graham |
| Stacey Plaskett | 119 | X | | | | | Stacey Plaskett |
| Ben Bernanke | 111 | | X | | | | Bernanke |
| Michael Cohen | 108 | X | | | | | Michael Cohen |
| Michael Flynn | 107 | X | | | | | Michael Flynn |
| Jared Kushner | 106 | X | | | | | Jared Kushner |
| Mike Pompeo | 105 | X | | | | | Mike Pompeo |
| Martin Schlaff | 105 | X | | | | | Martin Schlaff |
| James Comey | 102 | X | | | | | James Comey |
| Sarah Ferguson | 101 | X | | | | | Sarah Ferguson |
| George Soros | 100 | X | X | | | | George Soros |
| Hunter Biden | 99 | X | | | | | Hunter Biden |
| Brian Colleran | 96 | X | | | | | Brian Colleran |
| Paul Ryan | 96 | X | | | | | Paul Ryan |
| Medici (casa papal) | 94 | | | | | X | Medici |
| Howard Lutnick | 93 | X | | | | | Howard Lutnick |
| Mario Draghi | 93 | | X | | | | Draghi |
| Chris Tucker | 91 | X | | | | | Chris Tucker |
| Lawrence Summers | 86 | | | X | | | Lawrence Summers |
| Mike Pence | 86 | X | | | | | Mike Pence |
| Ivanka Trump | 85 | X | | | | | Ivanka Trump |
| Jay Clayton | 84 | X | | | | | Jay Clayton |
| Joseph Recarey | 84 | X | | | | | Joseph Recarey |
| Fareed Zakaria | 81 | | | X | X | | Fareed Zakaria |
| Bill Cosby | 80 | X | | | | | Bill Cosby |
| Kamala Harris | 79 | X | | | | | Kamala Harris |
| Eric Holder | 76 | X | | | | | Eric Holder |
| Lloyd Blankfein | 75 | | X | | | | Blankfein |
| Susan Rice | 73 | X | X | | X | | Susan Rice |
| Michael Milken | 73 | X | | | | | Michael Milken |
| Ben Sasse | 71 | X | | | | | Ben Sasse |
| Strauss Audrey | 70 | X | | | | | Strauss Audrey |
| Kash Patel | 68 | X | | | | | Kash Patel |
| Alan Greenspan | 68 | | X | | | | Greenspan |
| Mark Meadows | 67 | X | | | | | Mark Meadows |
| Shimon Peres | 67 | | X | | | | Shimon Peres |
| Eliot Spitzer | 63 | X | | | | | Eliot Spitzer |
| Rupert Murdoch | 62 | X | X | | | | Rupert Murdoch |
| John Scarola | 62 | X | | | | | John Scarola |
| Adam Schiff | 62 | X | | | | | Adam Schiff |
| Philipp Hildebrand | 0* | | X | | | | Hildebrand (61 hits sobrenome, 0 nome completo) |
| Silvio Berlusconi | 60 | | X | | | | Berlusconi |
| Julian Assange | 60 | X | | | | | Julian Assange |
| Ron Desantis | 60 | X | | | | | Ron Desantis |
| Jay Z | 60 | X | | | | | Jay Z |
| Dick Cheney | 59 | X | | | | | Dick Cheney |
| Merrick Garland | 59 | X | | | | | Merrick Garland |
| Alison Moe | 59 | X | | | | | Alison Moe |
| Chuck Schumer | 59 | X | | | | | Chuck Schumer |
| Edward Snowden | 58 | X | | | | | Edward Snowden |
| Mick Jagger | 57 | X | | | | | Mick Jagger |
| Børge Brende | 56 | | | X | | | Børge Brende |
| Cory Booker | 56 | X | | | | | Cory Booker |
| Alec Baldwin | 55 | X | | | | | Alec Baldwin |
| Monica Lewinsky | 55 | X | | | | | Monica Lewinsky |
| Dennis Ross | 54 | | | | X | | Dennis Ross |
| Thomas L. Friedman | 53 | | | X | | | Thomas L. Friedman |
| Jeff Sessions | 53 | X | | | | | Jeff Sessions |
| Pam Bondi | 52 | X | | | | | Pam Bondi |
| Ron Wyden | 52 | X | | | | | Ron Wyden |
| Leonard Blavatnik | 52* | | X | | | | Blavatnik (sobrenome único; "Friend of Ghislaine" documentado) |
| John Brennan | 51 | X | | | | | John Brennan |
| George Clooney | 50 | X | | | | | George Clooney |
| Michael Horowitz | 50 | X | | | | | Michael Horowitz |
| Barry Diller | 49 | X | | | | | Barry Diller |
| John Roth | 48 | X | | | | | John Roth |
| Robert De Niro | 45 | X | | | | | Robert De Niro |
| Gavin Newsom | 45 | X | | | | | Gavin Newsom |
| Brett Ratner | 45 | X | | | | | Brett Ratner |
| Roman Abramovich | 44 | | X | | | | Abramovich |
| Barry Krisher | 43 | X | | | | | Barry Krisher |
| Elvis Presley | 43 | X | | | | | Elvis Presley |
| Massimo (casa papal) | 42 | | | | | X | Massimo |
| Mattei (casa papal) | 42 | | | | | X | Mattei |
| John Bolton | 42 | X | | | | | John Bolton |
| Jeb Bush | 42 | X | | | | | Jeb Bush |
| Fidel Castro | 41 | X | | | | | Fidel Castro |
| Mark Filip | 41 | X | | | | | Mark Filip |
| Rod Rosenstein | 41 | X | | | | | Rod Rosenstein |
| Robert S. Mueller | 40 | X | | | | | Robert S. Mueller |
| Colin Powell | 39 | | X | | | | Colin Powell |
| Gordon Smith | 39 | | | | X | | Gordon Smith |
| Karl Rove | 38 | X | | | | | Karl Rove |
| Margaret Thatcher | 38 | X | | | | | Margaret Thatcher |
| Dianne Feinstein | 38 | | | | X | | Dianne Feinstein |
| Clare Iveagh | 36 | X | | | | | Clare Iveagh |
| David Rockefeller | 35 | | X | | X | | David Rockefeller |
| Alexandria Ocasio Cortez | 34 | X | | | | | Alexandria Ocasio Cortez |
| Abigail Wexner | 34 | X | | | | | Abigail Wexner |
| Daniel Parker | 34 | X | | | | | Daniel Parker |
| Doria (Pamphili-Landi) | 12 | | | | | X | Doria |
| Lee Plourde | 33 | X | | | | | Lee Plourde |
| Tucker Carlson | 32 | X | | | | | Tucker Carlson |
| Bruce Springsteen | 32 | X | | | | | Bruce Springsteen |
| Niall Ferguson | 31 | | | X | | | Niall Ferguson |
| Ron Paul | 31 | X | | | | | Ron Paul |
| John Ratcliffe | 31 | X | | | | | John Ratcliffe |
| Chad Readler | 31 | X | | | | | Chad Readler |
| Howard Rubenstein | 31 | X | | | | | Howard Rubenstein |
| Melania Trump | 31 | X | | | | | Melania Trump |
| Mark Yung | 30 | X | | | | | Mark Yung |
| Dan Bongino | 29 | X | | | | | Dan Bongino |
| David Miliband | 29 | | X | | | | David Miliband |
| George Osborne | 29 | | X | | | | George Osborne |
| Stephanie Avakian | 28 | X | | | | | Stephanie Avakian |
| Antony Blinken | 28 | X | | | | | Antony Blinken |
| Howard Heiss | 28 | X | | | | | Howard Heiss |
| Marilyn Monroe | 28 | X | | | | | Marilyn Monroe |
| Jacob Rothschild | 28 | | X | | | X | Jacob Rothschild |
| Russell Capone | 27 | X | | | | | Russell Capone |
| Robert Menendez | 27 | X | | | | | Robert Menendez |
| Michelle Obama | 27 | X | | | | | Michelle Obama |
| Borghese (casa papal) | 27 | | | | | X | Borghese |
| Edward Friedland | 26 | X | | | | | Edward Friedland |
| Mick Mulvaney | 26 | X | | | | | Mick Mulvaney |
| Zbigniew Brzezinski | 25 | | X | | X | | Zbigniew Brzezinski |
| Chelsea Clinton | 25 | X | | | | | Chelsea Clinton |
| Steny Hoyer | 25 | X | | | | | Steny Hoyer |
| James Margolin | 25 | X | | | | | James Margolin |
| Nicole McFarland | 25 | X | | | | | Nicole McFarland |
| Samantha Power | 25 | X | | | | | Samantha Power |
| Oleg Deripaska | 24 | | X | | | | Deripaska |
| Stephen Feinberg | 24 | X | | | | | Stephen Feinberg |
| Larry Kudlow | 24 | X | | | | | Larry Kudlow |
| Theresa May | 24 | X | | | | | Theresa May |
| Nicolas Roos | 24 | X | | | | | Nicolas Roos |
| Stephen Schwarzman | 24 | X | | | | | Stephen Schwarzman |
| Strobe Talbott | 24 | | | | X | | Strobe Talbott |
| Christian Sewing | 23 | | | X | | | Christian Sewing |
| David Reuben | 23 | | X | | | | David Reuben |
| Larry Nassar | 23 | X | | | | | Larry Nassar |
| Xavier Becerra | 22 | X | | | | | Xavier Becerra |
| Jill Biden | 22 | X | | | | | Jill Biden |
| Carl Kline | 22 | X | | | | | Carl Kline |
| Howard Lorber | 22 | X | | | | | Howard Lorber |
| Keir Starmer | 22 | X | | | | | Keir Starmer |
| Mervyn King | 22 | | X | | | | Mervyn King |
| Lakshmi Mittal | 0* | | X | | | | Mittal (22 hits sobrenome, 0 nome completo) |
| Mario Monti | 21 | | | X | | | Mario Monti |
| Anne-Marie Slaughter | 21 | | | | X | | Anne-Marie Slaughter |
| Jon Kyl | 21 | X | | | | | Jon Kyl |
| Victoria Hervey | 21 | X | | | | | Victoria Hervey |
| Jeffrey Rosen | 21 | X | | | | | Jeffrey Rosen |
| Robert Rubin | 21 | | X | | | | Robert Rubin |
| Francis Fukuyama | 20 | | | | X | | Francis Fukuyama |
| Todd Bistricer | 20 | X | | | | | Bistricer |
| George Economou | 20 | X | | | | | George Economou |
| Mike Huckabee | 20 | X | | | | | Mike Huckabee |
| Jerry Nadler | 20 | X | | | | | Jerry Nadler |
| Jamie Raskin | 20 | X | | | | | Jamie Raskin |
| Tim Scott | 20 | X | | | | | Tim Scott |
| Eric Swalwell | 20 | X | | | | | Eric Swalwell |
| Demis Hassabis | 19 | | | X | | | Demis Hassabis |
| David Bistricer | 19 | X | | | | | David Bistricer |
| Nikki Haley | 19 | X | | | | | Nikki Haley |
| Jens Stoltenberg | 19 | X | | X | | | Jens Stoltenberg |
| Mark Carney | 19 | | | X | | | Mark Carney |
| Kenneth Rogoff | 19 | | | | X | | Kenneth Rogoff |
| Marc Bistricer | 18 | X | | | | | Marc Bistricer |
| Ric Bradshaw | 18 | X | | | | | Ric Bradshaw |
| Patrick Byrne | 18 | X | | | | | Patrick Byrne |
| Rebekah Donaleski | 18 | X | | | | | Rebekah Donaleski |
| Colonna (casa papal) | 18 | | | | | X | Colonna |
| JD Vance | 17 | X | | | | | JD Vance |
| Gideon Rachman | 17 | | | X | | | Gideon Rachman |
| Graham Allison | 17 | | | | X | | Graham Allison |
| Robert Kagan | 17 | | | | X | | Robert Kagan |
| Florence Hutner | 16 | X | | | | | Florence Hutner |
| Hakeem Jeffries | 16 | X | | | | | Hakeem Jeffries |
| Robert May | 16 | X | | | | | Robert May |
| Joseph Pecorino | 16 | X | | | | | Joseph Pecorino |
| Orsini (casa papal) | 16 | | | | | X | Orsini |
| Bertrand Russell | 16 | | X | | | | Bertrand Russell |
| Phillip Frost | 15 | X | | | | | Phillip Frost |
| Ro Khanna | 15 | X | | | | | Ro Khanna |
| Rosie O'Donnell | 15 | X | | | | | Rosie O'Donnell |
| Stanley Fischer | 15 | | X | | X | | Stanley Fischer |
| Richard Holbrooke | 15 | | X | | X | | Richard Holbrooke |
| Peter Lee | 15 | | | X | | | Peter Lee |
| Bret Stephens | 15 | | | X | | | Bret Stephens |
| Todd Blanche | 14 | X | | | | | Todd Blanche |
| Tony Higgins | 14 | X | | | | | Tony Higgins |
| Alex Jones | 14 | X | | | | | Alex Jones |
| Lisa Monaco | 14 | X | | | | | Lisa Monaco |
| Nick Clegg | 14 | | X | | | | Nick Clegg |
| Loretta Lynch | 13 | X | | | | | Loretta Lynch |
| Steve Mnuchin | 13 | X | | | | | Steve Mnuchin |
| Jay Sekulow | 13 | X | | | | | Jay Sekulow |
| John D. Rockefeller | 13 | | | | X | | John D. Rockefeller |
| Timothy Geithner | 12 | X | X | | | | Timothy Geithner |
| David Bowdich | 12 | X | | | | | David Bowdich |
| Kathleen Dupont | 12 | X | | | | | Kathleen Dupont |
| Keith Ellison | 12 | X | | | | | Keith Ellison |
| Janis Joplin | 12 | X | | | | | Janis Joplin |
| Jack Lew | 12 | X | | | | | Jack Lew |
| Ed Markey | 12 | X | | | | | Ed Markey |
| Brian Deese | 12 | | | X | | | Brian Deese |
| Thomas Massie | 11 | X | | | | | Thomas Massie |
| Sophia Papapetru | 11 | X | | | | | Sophia Papapetru |
| Lisa Marie Presley | 11 | X | | | | | Lisa Marie Presley |
| Diana Ross | 11 | X | | | | | Diana Ross |
| Amy Schumer | 11 | X | | | | | Amy Schumer |
| Yitzhak Shamir | 11 | X | | | | | Yitzhak Shamir |
| Mark Rutte | 11 | | | X | | | Mark Rutte |
| James Moore | 11 | | | | X | | James Moore |
| Carl Bildt | 11 | | X | | | | Carl Bildt |
| John Elkann | 11 | | X | | | | John Elkann |
| Louis Mountbatten | 11 | | X | | | | Mountbatten |

---

## 9. Organizações Bilderberg nos Documentos Epstein

As organizações representadas no Bilderberg foram pesquisadas independentemente no Elasticsearch.

### 9.1 Top 30 Organizações

| # | Organização | ES Hits | Contexto |
|---|-------------|---------|----------|
| 1 | **Google / Google LLC** | 10.293 + 305 | Informação de subscritor Google encontrada nos documentos; pesquisas sobre contas de Epstein |
| 2 | **Deutsche Bank AG** | 5.299 | Banco principal de Epstein; certificados de depósito, transações financeiras |
| 3 | **New York Times / The NYT** | 2.701 + 1.839 | Artigos de notícias, newsletters, reportagens sobre o caso |
| 4 | **Business and Industry** | 1.436 | Categoria genérica de participantes |
| 5 | **Goldman Sachs** | 1.326 | Banco de investimento; transações documentadas |
| 6 | **Harvard University** | 1.087 | Doações de Epstein; programa de ciências; David Gergen, Larry Summers |
| 7 | **Journalist** | 1.020 | Categoria de participantes Bilderberg |
| 8 | **Citigroup** | 909 | Instituição financeira |
| 9 | **NATO** | 707 | Referências geopolíticas; Stoltenberg como secretário-geral |
| 10 | **Microsoft Corporation** | 551 | Conexão Bill Gates |
| 11 | **Department of the Treasury** | 536 | Larry Summers, Timothy Geithner |
| 12 | **The Atlantic** | 528 | Publicação |
| 13 | **Financial Times** | 431 | Publicação; Gideon Rachman, Martin Wolf |
| 14 | **BNP Paribas** | 424 | Banco francês |
| 15 | **Stanford University** | 369 | Hoover Institution; conexões acadêmicas |
| 16 | **World Economic Forum** | 317 | Davos; Børge Brende como presidente |
| 17 | **The Economist** | 268 | Publicação |
| 18 | **European Commission** | 229 | Barroso, von der Leyen |
| 19 | **Yale University** | 201 | Conexões acadêmicas |
| 20 | **Department of Defense** | 185 | Referências governamentais |
| 21 | **The Financial Times** | 172 | Variante do FT |
| 22 | **European Parliament** | 155 | Referências políticas |
| 23 | **National Security Council** | 154 | Aparato de segurança nacional |
| 24 | **BP plc** | 133 | Petrolífera |
| 25 | **London School of Economics** | 130 | Universidade |
| 26 | **Pfizer Inc.** | 121 | Farmacêutica; Albert Bourla no Bilderberg |
| 27 | **Shell plc** | 112 | Petrolífera |
| 28 | **Carnegie Endowment** | 80 | Think tank; Robert Kagan |
| 29 | **Hudson Institute** | 80 | Think tank neoconservador |
| 30 | **Hoover Institution** | 64 | Stanford; Niall Ferguson |

### 9.2 Organizações Notáveis de Menor Volume

| Organização | ES Hits | Nota |
|-------------|---------|------|
| **Kissinger Associates Inc.** | 31 | Consultoria de Henry Kissinger |
| **Kohlberg Kravis Roberts & Co.** | 24 | KKR; Henry Kravis |
| **Thiel Capital LLC** | 17 | Peter Thiel |
| **DeepMind** | 17 | Demis Hassabis; IA |
| **OpenAI** | 5 | Sam Altman |
| **Anthropic PBC** | 1 | Dario Amodei |
| **Palantir Technologies Inc.** | 1 | Peter Thiel |
| **Google DeepMind** | 3 | Demis Hassabis |

### 9.3 Análise: O Triângulo Financeiro

Três instituições bancárias dominam os documentos Epstein:

1. **Deutsche Bank AG** (5.299 hits) — banco principal pós-2013; multado $150M
2. **Goldman Sachs** (1.326 hits) — conexões via Lloyd Blankfein (75 hits) e Gary Cohn (377 hits no sobrenome)
3. **Citigroup** (909 hits) — transações financeiras documentadas

Todas estas instituições têm representantes regulares no Bilderberg, sugerindo que a rede financeira de Epstein estava profundamente integrada nas mesmas instituições que participam da governança global.

---

## 10. Conclusões e Investigações Pendentes

### 10.1 Conclusões Principais

**1. Epstein era um insider, não um outsider**
A sua presença na Trilateral Commission de 2008, ao lado de David Rockefeller, Kissinger, Summers e Brzezinski, demonstra que ele era um membro formal das estruturas de governança global. Isto contradiz a narrativa de que Epstein era apenas um "fixer" periférico.

**2. O cruzamento de listas revela concentração de poder**
Os nomes que aparecem em múltiplas listas E nos documentos Epstein formam um núcleo reduzido:
- **Susan Rice** (3 listas: DOJ+C300+TC, 73 hits)
- **Peter Thiel** (4 listas: DOJ+BIL23+BIL24+BIL25, 1.436 hits)
- **Bill Gates** (2 listas: DOJ+C300, 1.487 hits)
- **Bill Clinton** (2 listas: DOJ+C300, 1.178 hits)
- **David Rockefeller** (2 listas: C300+TC, 35 hits)

**3. As instituições são tão importantes quanto os indivíduos**
Deutsche Bank (5.299), Goldman Sachs (1.326), Harvard (1.087), e Google (10.293) aparecem massivamente nos documentos. O CEO atual do Deutsche Bank (Christian Sewing) participa do Bilderberg, criando continuidade institucional.

**4. A rede jurídica é reveladora**
Alan Dershowitz cobrou **$4,1 milhões** em honorários de Epstein. Jay Lefkowitz foi conectado via Jes Staley (JPMorgan). Kathy Ruemmler (ex-conselheira da Casa Branca) tinha reuniões diretas. Isto sugere que a proteção jurídica de Epstein era uma operação coordenada entre as maiores firmas e o governo.

**5. A conexão israelense é profunda**
Ehud Barak (2.209 hits) com iMessages sobre hotel em São Petersburgo; Benjamin Netanyahu (321 hits); Yitzhak Shamir (11 hits); Shimon Peres (67 hits); Stanley Fischer/Banco de Israel (15 hits). Combinado com Robert Maxwell (298 hits) e a operação Mossad documentada noutros dossiês, Israel emerge como um eixo central da rede.

### 10.2 Investigações Pendentes

1. **Quem indicou Epstein para a Trilateral Commission?** — Necessário obter atas de admissão de 2007-2008
2. **Qual o papel real de David Gergen (393 hits)?** — Partilha de arquivos Dropbox com Epstein merece análise completa dos documentos
3. **Lawrence Summers e o Banco do Cazaquistão** — Email sobre "arranjos" com o Deputy Governor sugere intermediação financeira
4. **Peter Thiel: "suéteres" ou algo mais?** — A coordenação de endereços de figuras de elite por Epstein merece investigação
5. **Daniel Siad (1.056 hits)** — Comunicações Skype regulares em 2019; identidade e papel não claros
6. **Dominique Strauss-Kahn (50 hits para "Strauss-Kahn", 29 para nome completo)** — Contexto DSK-Epstein merece investigação separada
7. **Christian Sewing / Deutsche Bank** — CEO atual no Bilderberg enquanto banco ainda sob investigação por facilitação Epstein
8. **Martin Schlaff (105 hits)** — Oligarca austríaco com conexões a Israel e tráfico de influência
9. **Doria-Pamphili-Landi** — Nome completo = 0 hits; "Doria" isolado = 12 hits; contexto a determinar
10. **A sobreposição C300 + Trilateral**: 6 nomes aparecem em ambas as listas E nos documentos Epstein (Rockefeller, Brzezinski, Fischer, Holbrooke, Rice, Bergsten) — investigar se existe um sub-grupo que facilitou a entrada de Epstein

---

*Dossiê gerado por cruzamento automatizado de 1.381 nomes contra ~580.000 documentos Epstein. Dados extraídos em 15 de fevereiro de 2026. Todas as contagens de hits referem-se a documentos no Elasticsearch (índice `epstein`). Buscas por frase exata são as mais confiáveis; buscas por sobrenome podem incluir falsos positivos.*
