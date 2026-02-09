# DOSSIE: PANDEMIA, BILL GATES E A REDE CIENTIFICA DE JEFFREY EPSTEIN

**Data**: 6 de fevereiro de 2026
**Versao**: 1.0
**Investigador**: Leonardo Dias / Arvor
**Metodologia**: Analise sistematica do indice Elasticsearch `epstein` (Datashare, 384.890 documentos), grafo Neo4j (1.3 milhao de nos, 5.5 milhoes de relacionamentos), leitura integral de documentos primarios, cross-reference com fontes publicas
**Classificacao**: Investigacao Jornalistica
**Status**: VERIFICADO com documentos primarios. Cada afirmacao tem documento-fonte identificado

---

## 1. RESUMO EXECUTIVO

Jeffrey Epstein construiu, ao longo de pelo menos uma decada, uma rede de relacionamentos cientificos que incluia pesquisadores de ponta em genetica, biologia sintetica, virologia e previsao de pandemias. No centro dessa rede, Bill Gates manteve com Epstein um relacionamento profundo e continuado entre 2010 e 2017, documentado por dezenas de jantares, emails trilaterais e planos financeiros conjuntos.

O nexo entre Gates e Epstein era Boris Nikolic, chefe do think tank privado de Gates (BGC3) e posteriormente nomeado executor testamentario do proprio Epstein. Nikolic intermediou reunioes, encaminhou informacoes e serviu de ponte entre o universo Gates e o universo Epstein de maneira documentalmente inequivoca.

Em paralelo, Nathan Wolfe, fundador da empresa de previsao de pandemias Metabiota (anteriormente Global Viral Forecasting), frequentava a residencia de Epstein e lhe enviava referencias academicas sobre questionarios de comportamento sexual e rastreamento de DSTs. George Church, professor de Genetica em Harvard e pioneiro do CRISPR, mantinha contato regular com Epstein e lhe forneceu pesquisas sobre rejuvenescimento. Epstein financiou conferencias de biologia sintetica e virologia com participantes como Craig Venter (Projeto Genoma Humano) e Eric Lander (Broad Institute).

Em maio de 2017, um email encaminhado ao endereco pessoal de Epstein detalhava os "deliverables" do BGC3 para Gates, incluindo especificacoes tecnicas para "Strain pandemic simulation" e um whitepaper sobre "neurotechnologies as weapons in national intelligence and defense".

Este dossie nao encontrou evidencia direta de que Epstein tenha financiado pesquisa de criacao de pandemias ou armas biologicas. O que os documentos revelam e algo diverso e, a seu modo, igualmente perturbador: um pedofilo condenado posicionado no exato ponto de interseccao entre riqueza (Gates, JPMorgan, Leon Black), ciencia de fronteira (Church, Wolfe, Venter, Lander) e poder politico (Comite do Nobel, Nacoes Unidas), usando cada eixo para amplificar os demais, enquanto desenvolvia, em paralelo, planos documentados de eugenia e inseminacao de mulheres em seu rancho no Novo Mexico.

**Contagem de referencias no corpus**:

| Termo | Hits | Contexto predominante |
|-------|------|-----------------------|
| Bill Gates | 354 | Comunicacoes diretas + noticias |
| Gates (total) | 1.022 | Inclui K&L Gates (escritorio advocacia) |
| Boris Nikolic | 1.334 | Comunicacoes diretas |
| George Church | 453 | Comunicacoes diretas |
| Nathan Wolfe | 69 | Comunicacoes diretas |
| pandemic | 315 | Maioria noticias COVID; 2 a 3 emails diretos |
| vaccine | 147 | Maioria artigos de imprensa |
| synthetic biology | 31 | Agendas de conferencia |
| eugenics | 22 | Artigos + discussoes pessoais |
| Gates Foundation | 84 | Esquema DAF + noticias |
| Terje Rod-Larsen | 312 | Comunicacoes diretas |

---

## 2. METODOLOGIA

### 2.1 Fontes Primarias

- **Elasticsearch**: Indice `epstein` no Datashare (384.890 documentos, Elasticsearch 7.17.9)
- **Neo4j**: Grafo com 1.3 milhao de nos e 5.5 milhoes de relacionamentos
- **Tipos de documento**: Emails internos, agendas, registros financeiros, documentos judiciais, deposicoes, artigos de imprensa incorporados ao acervo

### 2.2 Tecnicas de Busca

- `match` para termos simples, `match_phrase` para termos compostos (licao critica: `match: "Bill Gates"` retorna "Bill" OR "Gates"; `match_phrase` retorna a frase exata)
- `bool.must` para cruzamento de termos
- `highlight` com `fragment_size: 300` para contextualizacao
- Analise em lote com Python para classificacao e desduplicacao

### 2.3 Ressalvas Metodologicas

1. **"pandemic" inflado**: Dos 315 hits de "pandemic", mais de 300 sao artigos juridicos sobre o impacto da COVID nos processos Epstein, NAO comunicacoes diretas de Epstein sobre pandemias
2. **"Gates" inflado**: O escritorio de advocacia K&L Gates aparece frequentemente, inflando a contagem para 1.022
3. **"WHO" inutilizavel**: 35.237 hits porque "who" e pronome interrogativo em ingles
4. **Wuhan, gain of function, EcoHealth, bioweapon**: Hits provem de artigos de imprensa no corpus, nao de comunicacoes de Epstein
5. **Conexoes sao PESSOAIS, nao institucionais**: O que conecta Gates a Epstein e a rede de pessoas (Nikolic, Wolfe, Church), nao financiamento direto de pesquisa pandemica
6. **O trabalho da Gates Foundation com vacinas e publico e mainstream**: A conexao com Epstein e sobre a rede de pessoas, nao sobre o programa de vacinacao em si

---

## 3. A RELACAO GATES-EPSTEIN: CRONOLOGIA DOCUMENTADA

A relacao entre Bill Gates e Jeffrey Epstein produziu 354 mencoes diretas a "Bill Gates" no corpus de documentos. O que segue e a cronologia reconstruida a partir de emails, agendas e registros internos. Cada entrada tem documento-fonte verificado.

### 3.1 Novembro-Dezembro 2010: O Inicio

**28 de novembro de 2010** (EFTA02414311)
Email de Epstein coordenando jantar para 6 de dezembro:

> "6th now.. girls should be form 5-7 gates from 7-"

**ANALISE**: A formulacao e reveladora. "Girls" das 17h as 19h, Gates chegando as 19h. Sugere que Epstein organizava a presenca de mulheres antes da chegada de Gates, ou que havia atividades separadas. O termo "girls" no vocabulario operacional de Epstein e consistente com o uso documentado em outros contextos.

**2 de dezembro de 2010** (EFTA02410629)
Gates cancela o jantar de 6 de dezembro. Email enviado do endereco **billg@bgc3.com** (confirmando que Gates usava email corporativo do BGC3 para se comunicar com Epstein):

> "Nathan had agreed with you that I would enjoy meeting with him and that it is a fine thing to do so on another trip I will try and do it."

**ANALISE**: Gates menciona "Nathan" como intermediario, isto e, alguem que concordou com Epstein sobre o encontro. Este "Nathan" pode ser Nathan Wolfe ou Nathan Myhrvold. O tom e de familiaridade e promessa de futuro encontro.

### 3.2 Janeiro-Fevereiro 2011: Jantares na 71st Street

**28 de janeiro de 2011** (EFTA02320660)
Email interno da equipe de Epstein:

> "Bill Gates and Boris Nikolic will be coming back for dinner on Tuesday Feb. 1st around 8pm. Peter Mandelson will be arriving that evening as well"

**NOTA**: Peter Mandelson e ex-Secretario de Estado britanico e membro da Camara dos Lordes. A presenca dele, de Gates e de Nikolic num jantar na residencia de Epstein na E 71st Street indica o nivel de acesso politico que esses jantares proporcionavam.

**1 de fevereiro de 2011** (EFTA02320685)
Confirmacao do jantar:

> "Bill Gates and Boris Nikolic is coming for dinner at 71st this Monday and Tuesday night.. both nights!"

**ANALISE**: Duas noites consecutivas. Nao se trata de um encontro casual ou uma reuniao de negocios pontual. Gates e Nikolic jantaram na residencia de um pedofilo condenado (Epstein foi condenado em 2008) duas noites seguidas.

### 3.3 Maio 2011: "Power Dinner"

**2 de maio de 2011** (EFTA02320203)
Email de coordenacao:

> "dinner Monday night is at 9pm. Bill Gates, Larry Summers and Jes Staley are the attendees at the moment. Power dinner!!"

**ANALISE**: A expressao "Power dinner!!" nao e acidental. Gates (Microsoft/Gates Foundation), Larry Summers (ex-Secretario do Tesouro, presidente de Harvard) e Jes Staley (CEO do JPMorgan Private Bank, depois CEO do Barclays). Tres das pessoas mais influentes do mundo financeiro e politico americano, reunidas a mesa de Jeffrey Epstein, tres anos apos sua condenacao por crimes sexuais.

**NOTA SOBRE JES STALEY**: No diario de uma vitima de Epstein (EFTA02731469), "Mr. Staley" e descrito como abusador que "deixou marcas de cinto nos bracos" da vitima e a chamava de "tinkerbell". Staley renunciou do Barclays em 2021 apos investigacao sobre seus lacos com Epstein.

**NOTA SOBRE LARRY SUMMERS**: No mesmo diario (EFTA02731425), "Larry Summers" e descrito como "Fucking disgusting" no contexto de abuso.

### 3.4 Julho 2012: Gates na Noruega

**Julho de 2012** (EFTA02557253)
Lembrete:

> "Reminder Bill Gates in Norway Aug 6"

**ANALISE**: A Noruega e relevante por causa de Terje Rod-Larsen (ver Capitulo 11). Epstein rastreava os movimentos de Gates e coordenava encontros com o diplomata norueguês que lhe daria acesso ao Comite do Premio Nobel da Paz.

### 3.5 Janeiro 2012: Jes Staley Pede Acesso a Gates via Epstein

**Janeiro de 2012** (EFTA02548854)
O escritorio de Jes Staley solicita a Epstein:

> "1 on 1 meeting with Bill Gates next week while Jes is at Davos"

**ANALISE**: Epstein funcionava como broker de acesso. O CEO do banco mais poderoso do mundo pedia a um pedofilo condenado uma reuniao privada com Gates. Isso ilumina o poder real que Epstein exercia: nao era riqueza propria (cuja origem permanece obscura), mas a capacidade de conectar pessoas que, sem ele, nao se conectariam facilmente.

### 3.6 Fevereiro 2013: Almoco Gates + Senador Mitchell

**Fevereiro de 2013** (EFTA02565753)
Epstein pergunta sobre almoco com Gates e o Senador George Mitchell.

**NOTA SOBRE GEORGE MITCHELL**: No diario da vitima (EFTA02731431), Mitchell e descrito com as palavras: "You think would be good like a grandpa are bad." Mitchell era mediador do processo de paz na Irlanda do Norte e Enviado Especial para o Oriente Medio. Renunciou ao conselho da Universidade de New York apos as revelacoes sobre Epstein.

### 3.7 Janeiro 2014: Skype Call Organizada por Epstein

**28 de janeiro de 2014** (EFTA02395031, EFTA02356983)
Epstein organiza uma chamada de Skype entre Bill Gates e Larry Cohen.

**ANALISE**: Larry Cohen e uma figura recorrente na interseccao Gates-Epstein. Ele aparece como intermediario do esquema DAF (Donor Advised Fund), detalhado no Capitulo 10.

### 3.8 Marco 2014: Emails Trilaterais e Jantar com Reid Hoffman

**Marco de 2014** (EFTA02395937, EFTA02404769)
Multiplos emails de tres vias entre Epstein, Gates e Larry Cohen sobre o DAF (Donor Advised Fund) e um jantar com Reid Hoffman (fundador do LinkedIn).

**14 de marco de 2014** (EFTA00373841)
Agenda de Epstein mostra:

> "TBD Dinner w/Bill Gates"

### 3.9 Agosto-Setembro 2014: O Apice

**Agosto de 2014** (EFTA02587505)
Epstein escreve a Peter Thiel (cofundador do PayPal):

> "Bill Gates will be with me monday 8th in ny"

E no mesmo email:

> "head of nobel peace prize committee staying with me"

**ANALISE**: Epstein usava Gates como cartao de visita para atrair outras figuras poderosas, e vice-versa. O "head of nobel peace prize committee" e quase certamente conectado a Terje Rod-Larsen.

**Setembro de 2014** (EFTA00363562, EFTA00363580)
A agenda de Gates em torno de Epstein nesse periodo mostra uma sequencia de reunioes:
- Escritorio de Leon Black
- Larry Summers
- Mort Zuckerman (dono do US News & World Report)
- Kathy Ruemmler no Four Seasons

Todas com Bill Gates.

**25 de setembro de 2014** (EFTA02386397)
Email de Bill Gates PARA Epstein (com copia para Larry Cohen) sobre o DAF. Gates menciona:

> "seeing the President on budget and Ebola"

E um jantar com "Ray Dalio and Paul Tudor Jones" (dois dos maiores gestores de hedge funds do mundo).

**ANALISE**: Este email e particularmente significativo porque: (a) Gates escreve diretamente a Epstein, nao o contrario; (b) Gates compartilha com Epstein informacao sobre sua reuniao com o Presidente dos EUA sobre Ebola; (c) Gates menciona Dalio e Paul Tudor Jones, dois nomes do topo da piramide financeira global. O nivel de intimidade e confianca implicito nessa comunicacao e dificil de exagerar.

**NOTA SOBRE LEON BLACK**: No diario de uma vitima (EFTA02731427-28), Leon Black e acusado de violencia sexual durante 7 a 8 anos contra uma vitima que tinha 16 anos quando o abuso comecou. Leon Black pagou mais de $158 milhoes a Epstein. A vitima descreve mordidas que deixaram sangue no carpete.

### 3.10 Dezembro 2014

**5 de dezembro de 2014** (EFTA02356543)
Jes Staley pergunta a Epstein se a reuniao com Bill Gates no dia seguinte continua confirmada.

### 3.11 Maio 2017: O Email sobre Pandemia

**24 de maio de 2017** (EFTA02389903)
Email trilateral. Epstein escreve a **Bill Gates E Boris Nikolic**:

> "with the massive cuts in science coming, the Donor Advised Fund should be the counter balance."

Nikolic responde:

> "It might be a great path forward for some key areas such as Energy, pandemic etc."

**ANALISE**: Este e o email mais diretamente relevante para a questao pandemica. Nikolic, falando em nome do BGC3 (think tank de Gates), identifica "pandemic" como uma das areas-chave para o Donor Advised Fund que Epstein promovia. O email e de maio de 2017, dois anos e meio antes da pandemia de COVID-19.

### 3.12 A Avaliacao de Michael Wolff

**Artigo de Michael Wolff no corpus** (EFTA02342151):

> "It is Bill Gates who at the end of the summer began prodding Epstein to begin a process of public rehabilitation. Epstein has been advising Gates on a new way to increase the clout of the Gates Foundation by adding a constellation of other charitable funds that would be bundled with the Gates operation."

**ANALISE**: Segundo Wolff, a relacao era bidirecional. Gates queria a expertise financeira de Epstein para ampliar o alcance da Gates Foundation. Epstein queria a reputacao de Gates para sua reabilitacao publica. O DAF era o veiculo desenhado para servir a ambos os propositos simultaneamente.

---

## 4. BORIS NIKOLIC: O ELO BGC3-GATES-EPSTEIN

Boris Nikolic aparece 1.334 vezes no corpus de documentos. Destes, 733 o mencionam em conjunto com Epstein. Nikolic e, sem exagero documental, a pessoa que mais intensamente conecta o universo de Bill Gates ao universo de Jeffrey Epstein.

### 4.1 Quem e Boris Nikolic

- Cientista de formacao (imunologia)
- Ex-conselheiro cientifico de Bill Gates na Gates Foundation
- Diretor do BGC3 (Bill Gates Catalyst 3), o think tank privado de Gates
- Usava email bgc3.com em comunicacoes com Epstein
- Investidor em startups de biotecnologia apos sair do BGC3

### 4.2 Executor Testamentario de Epstein

**STATUS: VERIFICADO** | Documento: EFTA00060795

O testamento de Jeffrey Epstein, assinado dois dias antes de sua morte, designa:

> "I appoint BORIS NIKOLIC, as successor Executor"

A compensacao prevista: $250.000.

**Relatorio do FBI sobre Nikolic** (EFTA00128843):
Um relatorio de CHS (Confidential Human Source) do FBI confirma:

> "Nikolic was designated a executor of Jeffrey Epstein's estate"

**ANALISE**: Nikolic afirmou publicamente que a nomeacao o surpreendeu e que jamais aceitaria. Mas o fato de Epstein o ter escolhido como executor de ultima instancia do seu patrimonio indica um nivel de confianca que transcende reunioes de negocios casuais. Epstein, que mantinha relacoes com centenas de pessoas poderosas, escolheu o homem de Gates para administrar seu legado apos a morte.

### 4.3 Cronologia de Reunioes Nikolic-Epstein

Dezenas de emails de agendamento documentam reunioes regulares entre Nikolic e Epstein na residencia da E 71st Street, de 2010 a pelo menos 2017. Exemplos:

- **28 de janeiro de 2011**: Nikolic janta com Gates na residencia de Epstein (EFTA02320660)
- **1 de fevereiro de 2011**: Duas noites consecutivas (EFTA02320685)
- **Multiplas datas 2011-2017**: Emails de coordenacao de reunioes na E 71st Street

### 4.4 Nikolic como Intermediario

**Encaminhamento de informacoes sobre Principe Andrew** (EFTA02421641):
Nikolic encaminhou a Epstein informacoes sobre o Principe Andrew, indicando que ele filtrava noticias relevantes para Epstein.

**Pergunta sobre Nathan Wolfe** (EFTA02421017):
Nikolic perguntou a Epstein:

> "how was your mtg w Nathan?"

**ANALISE**: Nikolic sabia que Epstein se reunia com Nathan Wolfe (fundador da Metabiota) e acompanhava essas reunioes. A pergunta sugere que o encontro Epstein-Wolfe era de interesse para Nikolic e, por extensao, para o circulo Gates.

**Artigo sobre Gates encaminhado a Epstein** (EFTA02377958):
Nikolic encaminhou a Epstein um artigo do Wall Street Journal intitulado "This Man's Job: Make Bill Gates Richer".

**Viagem com Gates** (EFTA02571172):
Nikolic escreveu a Epstein:

> "awaiting my delayed flight to India where I am meeting Bill"

### 4.5 Nikolic no Triangulo Gates-Epstein-Pandemia

O email de 24 de maio de 2017 (EFTA02389903) em que Nikolic escreve sobre "pandemic" como area-chave para o DAF ja foi citado no Capitulo 3. E a evidencia documental mais direta de que a palavra "pandemic" foi usada em comunicacao trilateral Gates-Nikolic-Epstein.

---

## 5. NATHAN WOLFE: PANDEMIA, METABIOTA E COMPORTAMENTO SEXUAL

Nathan Wolfe aparece 69 vezes no corpus. A relevancia de Wolfe nao esta na quantidade de mencoes, mas na qualidade perturbadora do conteudo.

### 5.1 Quem e Nathan Wolfe

- Virologista americano, PhD em imunologia
- Fundador e CEO da Global Viral Forecasting (GVF), renomeada METABIOTA
- Missao declarada da Metabiota: "leader in research and services to predict and prevent pandemics"
- Membro do conselho do EcoHealth Alliance (organizacao no centro das investigacoes sobre gain-of-function)
- Autor do livro "The Viral Storm" (2011) sobre surgimento de pandemias
- Recebeu financiamento da DARPA, Google e da Gates Foundation

### 5.2 Relacao com Epstein

Wolfe mantinha relacao pessoal com Epstein, visitando-o regularmente em Florida e Nova York de 2009 a pelo menos 2013.

**Hospedagem e logistica** (EFTA02433195):
Epstein ofereceu a Wolfe:

> "apt available and a car for your use"

**ANALISE**: Epstein oferecia apartamento e carro a Wolfe na Florida. Este padrao de hospitalidade e identico ao que Epstein oferecia a mulheres transportadas (Deimante Sabaliauskaite, Arina, etc.). No caso de Wolfe, o contexto e profissional, mas a logistica de acolhimento e a mesma.

### 5.3 O Email sobre Comportamento Sexual e DSTs

**STATUS: VERIFICADO** | Documento: EFTA02378487

Nathan Wolfe enviou a Epstein referencias academicas sobre questionarios de comportamento sexual e rastreamento de DSTs:

> "Below are some references that show how sexual behavior questionnaires have been validated. I believe these issues have been well addressed and am not concerned that we can get good data on changes in sexual behavior within individuals over time in relation to variables like the incidence of new STIs."

Wolfe propôs um "cohort study" sobre comportamento sexual.

**ANALISE**: Este e um documento critico. Nathan Wolfe, especialista em pandemias, enviou a Jeffrey Epstein, pedofilo condenado, material academico validado sobre como monitorar mudancas no comportamento sexual ao longo do tempo em relacao ao surgimento de novas DSTs. As perguntas que se impoem:

1. Por que Epstein estaria interessado em rastrear comportamento sexual cientificamente?
2. Quem seria a coorte (cohort) desse estudo proposto?
3. Havia conexao entre esse estudo e as mulheres transportadas por Epstein?

Os documentos nao respondem a essas perguntas. Mas o fato de que um especialista em pandemias fornecia a um traficante sexual ferramentas cientificas para monitoramento de comportamento sexual e um achado documental que merece investigacao adicional.

### 5.4 Wolfe nas Conferencias Cientificas de Epstein

**STATUS: VERIFICADO** | Documento: EFTA02441292

Wolfe aparece na lista de participantes de conferencia cientifica financiada por Epstein sobre:

> "Evolutionary Code dynamics... virus dynamics"

Outros participantes da mesma conferencia: George Church, Eric Lander (Broad Institute, depois conselheiro cientifico de Biden), Martin Nowak (Harvard).

### 5.5 Metabiota no Corpus

O termo "Metabiota" aparece apenas 3 vezes no corpus, todas em referencias a empresa. Nao ha evidencia de financiamento direto de Epstein a Metabiota nos documentos.

---

## 6. GEORGE CHURCH: CRISPR, REJUVENESCIMENTO E EUGENIA

George Church aparece 453 vezes no corpus, um numero extraordinariamente alto para um academico. Church e professor de Genetica na Harvard Medical School, pioneiro do sequenciamento genomico e do CRISPR, e uma das figuras centrais da revolucao em edicao genetica.

### 6.1 Reunioes Regulares com Epstein

Church manteve reunioes regulares com Epstein entre pelo menos 2010 e 2018, documentadas em emails de agendamento. Locais incluiam a residencia de Epstein na E 71st Street e o instituto de Martin Nowak em Harvard.

**Anos com reunioes documentadas**: 2010, 2013, 2014, 2015, 2016, 2018.

**Transporte fornecido por Epstein** (EFTA02421924):
Servico de carro organizado para levar Church para casa apos visitas.

### 6.2 O PDF "Rejuvenate"

**STATUS: VERIFICADO** | Documentos: EFTA00353065, EFTA00353066

Lesley Groff (assistente executiva de Epstein) enviou email contendo:

> "Jeffrey requested the attached pdf"

O PDF anexado: "Rejuvenate", de autoria de George Church, sobre rejuvenescimento celular.

**ANALISE**: Epstein nao apenas se reunia com Church, mas solicitava ativamente material cientifico sobre rejuvenescimento. Combinado com o interesse documentado de Epstein em eugenia (ver Capitulo 7), o "Rejuvenate" de Church se insere num padrao mais amplo de fascinio por manipulacao genetica e extensao da vida.

### 6.3 Church, Epstein e Noam Chomsky

**STATUS: VERIFICADO** | Documento: EFTA00333751

Email confirmando reuniao:

> "George would gladly meet Jeffrey and Noam Chomsky on Saturday, at 1pm"

Local: Instituto de Martin Nowak em Harvard.

**STATUS: VERIFICADO** | Documento: EFTA00351424

Jantar confirmado:

> "Martin, George, Joscha and Noam Chomsky... dinner Mon. March 23 at Martin's Institute, 8pm"

**ANALISE**: Epstein reunia, no mesmo espaco fisico, o geneticista pioneiro do CRISPR (Church), o linguista mais citado do seculo XX (Chomsky), o matematico biologico de Harvard (Nowak) e pesquisadores de inteligencia artificial (Joscha Bach). Esses jantares nao eram sociais. Eram simposios privados de fronteira cientifica, organizados e financiados por um condenado por crimes sexuais.

### 6.4 Church e a Rede Biotech de Epstein

**STATUS: VERIFICADO** | Documento: EFTA00329744

Church conectou Epstein a:
- **Luhan Yang**: Pesquisadora de CRISPR
- **Geoff Mackay**: Executivo de biotecnologia

Church funcionava, assim, como ponte entre Epstein e a vanguarda da edicao genetica.

### 6.5 Church e a Questao da Eugenia

George Church admitiu publicamente, apos as revelacoes sobre Epstein, que nao tinha conhecimento da extensao dos crimes de Epstein. Mas documentos internos mostram que Church sabia do interesse de Epstein em eugenia:

- Participou de conferencias cujo tema incluia "biologia sintetica" e "dinamica de virus" (EFTA02441292)
- Forneceu pesquisa sobre rejuvenescimento a pedido pessoal de Epstein
- A eugenia e mencionada em pelo menos uma conversa da qual Church era potencial participante

---

## 7. O PROGRAMA DE EUGENIA DE EPSTEIN (ZORRO RANCH)

A eugenia nao era para Epstein uma curiosidade intelectual. Era um programa.

### 7.1 Evidencia Documental

**STATUS: VERIFICADO** | Documento: EFTA00069900

Artigo do New York Times preservado no corpus:

> "Epstein hoped to seed the human race with his DNA by impregnating women at his vast New Mexico ranch"

> "On multiple occasions starting in the early 2000s, Mr. Epstein told scientists and businessmen about his ambitions to use his New Mexico ranch as a base where women would be inseminated with his sperm"

> "Critics have likened transhumanism to a modern-day version of eugenics"

### 7.2 "Are We Ready for Eugenics?"

**STATUS: VERIFICADO** | Documento: EFTA02367335

Email a Epstein compartilhando artigo da revista Quadrant intitulado "Are We Ready for Eugenics?"

### 7.3 Discussao sobre "genius...and eugenics"

**STATUS: VERIFICADO** | Documento: EFTA02414772

Email discutindo "genius...and eugenics" com Martin Seligman, fundador da Psicologia Positiva e professor da Universidade da Pensilvania.

### 7.4 Verbete Enciclopedico

**STATUS: VERIFICADO** | Documento: EFTA00263107

Texto de formato enciclopedico nos documentos:

> "He addressed the scientific community at various events and occasions and communicated his fascination with eugenics"

### 7.5 O Diario da Vitima: "Superior Gene Pool" e "Baby Ranch"

Conforme documentado no dossie `dossie_diarios_vitima_programa_eugenia.md`, o diario de uma vitima (EFTA02731420, EFTA02731361, EFTA02731465) detalha:

- **"Superior Gene Pool"**: Epstein selecionava mulheres por cor de cabelo e olhos
- **"Perfect offspring"**: Bebes eram produzidos como parte de um programa eugenico
- **"Baby Ranch"**: O Zorro Ranch no Novo Mexico era o local central da operacao
- **Multiplas gravidezes forcadas**: Pelo menos 3 gravidezes, abortos forcados, bebes retirados
- **Conexao com Joao de Deus**: Email de dezembro de 2020 aos investigadores conectou o Zorro Ranch ao esquema de "baby farm" do curandeiro brasileiro (condenado a 370 anos). Assunto: "Woman who accused John of God cult leader of rape mysteriously kills herself at Spanish home"

**NOTA CRITICA**: O FBI nunca investigou o Zorro Ranch.

### 7.6 Termos Relacionados no Corpus

| Termo | Hits | Contexto |
|-------|------|----------|
| eugenics | 22 | Artigos + discussoes pessoais |
| seed the human race | 9 | Artigo do NYT |
| transhumanism | 10 | Artigos sobre Epstein |
| cryonics | 8 | Artigos sobre Epstein |
| CRISPR | 18 | Referencias cientificas |
| genetic engineering | 19 | Discussoes cientificas |
| DNA | 1.262 | Multiplos contextos |
| genome | 141 | Discussoes cientificas |
| Rejuvenate | 11 | Pesquisa de George Church |
| rejuvenation | 131 | Contextos mistos |

---

## 8. A REDE CIENTIFICA DE EPSTEIN: CONFERENCIAS E FINANCIAMENTO

### 8.1 Biologia Sintetica e Origens da Vida

**STATUS: VERIFICADO** | Documentos: Multiplos

Epstein financiou conferencias no ASU Origins Project sobre:

> "Origins of Life, and Synthetic Biology"

Participante de destaque: **Craig Venter**, lider do Projeto Genoma Humano privado.

Organizador: **Lawrence Krauss**, diretor do ASU Origins Project.

**NOTA SOBRE KRAUSS**: No diario da vitima (EFTA02731469), "Mr. Sauerkraut Krauss" e descrito como "Gross" (nojento) no contexto de abuso.

O termo "synthetic biology" aparece 31 vezes no corpus, todas conectadas a agendas de conferencias financiadas por Epstein.

### 8.2 Conferencia de Dinamica Viral

**STATUS: VERIFICADO** | Documento: EFTA02441292

Lista de participantes de conferencia sobre "Evolutionary Code dynamics... virus dynamics":

- **George Church** (Harvard, CRISPR)
- **Eric Lander** (Broad Institute/MIT, depois conselheiro cientifico de Biden)
- **Nathan Wolfe** (Global Viral Forecasting/Metabiota)
- **Martin Nowak** (Harvard, biologia matematica)

Epstein e listado como financiador da conferencia.

**ANALISE**: A presenca simultanea de Church (genetica), Wolfe (virologia pandemica), Lander (genomica) e Nowak (modelagem matematica de doencas) numa conferencia financiada por Epstein sobre "dinamica viral" e notavel. Esses nao eram cientistas marginais. Eram (e sao) figuras centrais da ciencia contemporanea.

### 8.3 Martin Nowak e o Programa de Biologia Evolutiva

Martin Nowak, professor de Biologia e Matematica em Harvard, dirigia o Programa de Dinamica Evolutiva. Epstein doou ao menos $6.5 milhoes ao programa de Nowak (conforme fontes publicas). O instituto de Nowak era o local fisico de reunioes entre Epstein, Church, Chomsky e outros.

### 8.4 O Padrao: Ciencia como Instrumento de Poder

Os documentos revelam um padrao consistente. Epstein nao estava apenas "interessado em ciencia". Ele:

1. **Financiava** conferencias e programas (Nowak, ASU Origins)
2. **Reunia** cientistas de ponta em encontros privados (Church, Wolfe, Lander, Venter, Chomsky)
3. **Solicitava** material cientifico especifico (Rejuvenate de Church, questionarios de comportamento sexual de Wolfe)
4. **Aplicava** conceitos cientificos a seus proprios programas (eugenia no Zorro Ranch)
5. **Usava** os cientistas como isco para atrair figuras de poder (Gates, Thiel)

---

## 9. BGC3 E "PANDEMIC SIMULATION"

### 9.1 O Documento

**STATUS: VERIFICADO** | Documento: EFTA02381427

Em 3 de marco de 2017, um email a Bill Gates detalha:

> "bgc3 Deliverables and Scope"

Os deliverables incluem:

1. **"Follow-up recommendations and/or technical specifications for Strain pandemic simulation"**
2. **"Whitepaper on Neurotechnologies as weapons in national intelligence and defense"**
3. **"Blueprint for zero knowledge proof-based digital system to secure private personal health information"**

O email foi encaminhado para **jeevacation@gmail.com**, endereco pessoal de Epstein.

### 9.2 Analise

Este documento e o mais citado em teorias conspiracionistas sobre a relacao Gates-Epstein-pandemia. E necessario rigor ao analisa-lo.

**O que o documento CONFIRMA**:
- O BGC3 (think tank de Gates) trabalhava em especificacoes tecnicas para simulacao de pandemias em 2017
- O BGC3 simultaneamente trabalhava em neurotecnologias como armas e em sistemas de informacao de saude pessoal
- O documento foi encaminhado ao email pessoal de Epstein
- Epstein tinha acesso a informacoes sobre os projetos internos do BGC3

**O que o documento NAO CONFIRMA**:
- Que Epstein participava do desenvolvimento dessas especificacoes
- Que a simulacao de pandemia era ilicita (simulacoes de pandemia sao ferramentas padrao de saude publica)
- Que havia conexao entre essa simulacao e a pandemia de COVID-19 (que comecaria quase 3 anos depois)
- Que Epstein financiava essas atividades do BGC3

**CONTEXTO IMPORTANTE**: Em outubro de 2019, a Gates Foundation co-financiou o exercicio "Event 201", uma simulacao de pandemia de coronavirus organizada pelo Johns Hopkins Center for Health Security e pelo World Economic Forum. Essa simulacao, realizada semanas antes da COVID-19 emergir, e frequentemente citada como premonitoria. O documento BGC3 de 2017 indica que o interesse de Gates em simulacao de pandemias e anterior ao Event 201 e era compartilhado, ao menos parcialmente, com o circulo de Epstein.

### 9.3 Nikolic e "Pandemic" no DAF

Combinando este documento com o email de maio de 2017 (EFTA02389903), onde Nikolic escreve "pandemic" como area-chave para o DAF, emerge um quadro em que a preparacao para pandemias era tema ativo nas conversas Gates-Nikolic-Epstein em 2017.

---

## 10. O ESQUEMA DAF (DONOR ADVISED FUND) GATES-EPSTEIN

O Donor Advised Fund (DAF) e o projeto financeiro conjunto mais elaborado entre Gates e Epstein documentado no corpus.

### 10.1 A Visao de Epstein

**STATUS: VERIFICADO** | Documento: EFTA01300940

Epstein escreve a Jes Staley (JPMorgan):

> "donor advised fund. you could tie it initially just to the gates program, minimum gift 100 million. it could then be opened up later. IT will be the largest foundation in the world... done right its 100 billion dollars in 2 years"

**ANALISE**: A ambicao e inequivoca. Epstein concebeu um fundo que comecaria atrelado ao programa Gates, com doacao minima de $100 milhoes, que se tornaria "a maior fundacao do mundo" e, "feito corretamente", acumularia $100 bilhoes em dois anos. Para efeito de comparacao, o patrimonio da Gates Foundation em 2014 era de aproximadamente $42 bilhoes.

### 10.2 "Project Molecule" (JPMorgan)

**STATUS: VERIFICADO** | Documento: EFTA01301114

O JPMorgan desenvolveu internamente o "Project Molecule":

> "The Gates & J.P. Morgan Charitable Giving Fund"

O documento detalha uma estrutura global para o fundo.

### 10.3 "Why Gates/Apollo"

**STATUS: VERIFICADO** | Documento: EFTA00315353

Documento intitulado "Why Gates/Apollo" enumera beneficios de participacao, incluindo:

> "You will join Bill and share his giving and investment experience"

**ANALISE**: O nome "Apollo" e uma referencia a Apollo Global Management, liderada por Leon Black, que pagou mais de $158 milhoes a Epstein. A convergencia Gates-JPMorgan-Apollo-Epstein num unico veiculo financeiro e um dos achados mais reveladores do corpus.

### 10.4 O Email de Gates sobre o DAF e Ebola

O ja citado email de 25 de setembro de 2014 (EFTA02386397), em que Gates escreve a Epstein sobre o DAF mencionando sua reuniao com o Presidente sobre "budget and Ebola", coloca o DAF no mesmo paragrafo que uma crise pandemica (Ebola).

### 10.5 Cronologia DAF

| Data | Evento | Documento |
|------|--------|-----------|
| 2013-2014 | Epstein propoe DAF a Jes Staley (JPM) | EFTA01300940 |
| Jan 2014 | Skype Gates-Cohen organizado por Epstein | EFTA02395031 |
| Mar 2014 | Emails trilaterais Epstein-Gates-Cohen sobre DAF | EFTA02395937, EFTA02404769 |
| Set 2014 | Gates escreve a Epstein sobre DAF, Ebola e o Presidente | EFTA02386397 |
| Mai 2017 | Epstein propoe DAF como "counterbalance"; Nikolic responde "pandemic" | EFTA02389903 |

---

## 11. TERJE ROD-LARSEN: O DIPLOMATA QUE CONECTOU GATES AO NOBEL

Terje Rod-Larsen aparece 312 vezes no corpus. Diplomata noruegues, ex-Secretario-Geral Adjunto da ONU, presidente do International Peace Institute (IPI) em Nova York. Sua funcao na rede Epstein era uma: abrir portas que nenhum dinheiro do mundo consegue comprar.

### 11.1 A Conexao Gates-Nobel

**STATUS: VERIFICADO** | Documentos: EFTA00020923, EFTA00030938

Investigacoes do jornal noruegues Dagens Naeringsliv revelaram:

> "how Epstein managed to get Bill Gates through the doors of the Nobel Peace Prize committee's leader in 2013"

A via de acesso: Terje Rod-Larsen.

**ANALISE**: Epstein usou Rod-Larsen para conectar Gates ao presidente do Comite do Nobel da Paz na Noruega. Rod-Larsen renunciou ao IPI apos a publicacao de mais de 40 artigos do Dagens Naeringsliv sobre sua relacao com Epstein. Devia $130.000 a Epstein.

### 11.2 Pandemia e Rod-Larsen

**STATUS: VERIFICADO** | Documento: EFTA02499005

Em 2 de junho de 2015, Epstein compartilha com Rod-Larsen um artigo da Vox sobre Bill Gates e pandemia de gripe.

**ANALISE**: Epstein disseminava o pensamento de Gates sobre pandemias dentro de sua rede diplomatica. Rod-Larsen, com acesso ao mais alto nivel da ONU e do Comite do Nobel, recebia de Epstein material sobre a visao pandemica de Gates.

### 11.3 Epstein a Peter Thiel sobre Rod-Larsen

No email de agosto de 2014 a Peter Thiel (EFTA02587505), Epstein menciona:

> "Bill Gates will be with me monday 8th in ny"

E:

> "head of nobel peace prize committee staying with me"

O "head of nobel peace prize committee" e a conexao Rod-Larsen, usada por Epstein como atrativo para Thiel.

---

## 12. TERMOS BIOMEDICOS NOS DOCUMENTOS

A seguinte tabela apresenta a contagem de termos biomedicos relevantes no corpus, com contextualizacao. E essencial distinguir entre comunicacoes diretas de Epstein e artigos de imprensa incorporados aos documentos.

### 12.1 Termos com Comunicacoes Diretas de Epstein

| Termo | Hits | Comunicacoes diretas | Contexto predominante |
|-------|------|---------------------|----------------------|
| Boris Nikolic | 1.334 | SIM (733 com Epstein) | Agendamento, intermediacao |
| George Church | 453 | SIM | Reunioes, pesquisa |
| Bill Gates | 354 | SIM (emails, agendas) | Jantares, DAF, reunioes |
| Terje Rod-Larsen | 312 | SIM | Diplomacia, Nobel |
| Nathan Wolfe | 69 | SIM | Visitas, pesquisa sexual |
| synthetic biology | 31 | SIM (agendas) | Conferencias financiadas |
| eugenics | 22 | SIM (emails, discussoes) | Programa Zorro Ranch |
| CRISPR | 18 | PARCIAL | Referencias cientificas |
| genetic engineering | 19 | PARCIAL | Discussoes |
| Rejuvenate | 11 | SIM (solicitado por Epstein) | PDF de Church |
| transhumanism | 10 | INDIRETO (artigos sobre Epstein) | Reportagens |
| seed the human race | 9 | INDIRETO (NYT) | Programa de eugenia |
| Metabiota | 3 | PARCIAL | Referencias a empresa |

### 12.2 Termos Predominantemente de Imprensa/Juridicos

| Termo | Hits | Comunicacoes diretas | Contexto predominante |
|-------|------|---------------------|----------------------|
| pandemic | 315 | 2 a 3 emails diretos | Noticias COVID sobre processos |
| COVID | 773 | NENHUMA | Processos juridicos durante pandemia |
| vaccine | 147 | NENHUMA | Artigos de imprensa |
| virus | 821 | PARCIAL (conferencias) | Misto: ciencia + noticias |
| coronavirus | 274 | NENHUMA | Artigos de imprensa |
| Gates Foundation | 84 | PARCIAL (DAF) | Esquema DAF + noticias |
| Melinda Gates | 82 | PARCIAL | Emails + noticias |
| Microsoft | 1.172 | PARCIAL | Diversos |
| Fauci | 84 | NENHUMA | Artigos de imprensa |
| NIH | 91 | PARCIAL | Grants + noticias |
| Wuhan | 29 | NENHUMA | Noticias sobre COVID |
| EcoHealth | 3 | NENHUMA | Artigos de imprensa |
| gain of function | 1 | NENHUMA | Artigo sobre depoimento de Fauci |
| bioweapon | 2 | NENHUMA | Artigos sobre Ebola |
| GAVI | 6 | NENHUMA | Noticias sobre COVAX |
| CEPI | 3 | NENHUMA | Artigos de imprensa |
| mRNA | 10 | NENHUMA | Noticias/cientifico |
| cryonics | 8 | INDIRETO | Artigos sobre Epstein |
| DNA | 1.262 | PARCIAL | Multiplos contextos |
| genome | 141 | PARCIAL | Discussoes cientificas |
| rejuvenation | 131 | PARCIAL | Mistos |
| Global Health | 49 | PARCIAL | Mistos |

### 12.3 Analise Critica das Contagens

**O que os numeros REVELAM**: Epstein mantinha comunicacoes diretas e regulares com cientistas de ponta (Church: 453, Nikolic: 1.334, Wolfe: 69) e com Gates (354). Esses nao sao numeros de mencoes passageiras. Sao volumes compativeis com relacionamentos profundos e continuados.

**O que os numeros NAO REVELAM**: Os termos mais sensacionais (Wuhan, gain of function, bioweapon, Fauci) nao tem nenhuma comunicacao direta com Epstein. Sao exclusivamente provenientes de artigos de imprensa que fazem parte do corpus documental por terem sido coletados durante os processos judiciais.

---

## 13. CONCLUSOES E ANALISE

### 13.1 O que e CONFIRMADO pelos documentos

1. **Bill Gates manteve relacao profunda e continuada com Epstein de pelo menos 2010 a 2017**, incluindo dezenas de jantares na residencia de um pedofilo condenado, emails trilaterais, planejamento financeiro conjunto (DAF) e coordenacao de reunioes com terceiros poderosos

2. **Boris Nikolic era o nexo operacional entre Gates e Epstein**. Usava email BGC3 para se comunicar com Epstein, intermediava informacoes, acompanhava reunioes de Epstein com cientistas, e foi nomeado executor testamentario de Epstein

3. **Nathan Wolfe, fundador de empresa de previsao de pandemias, mantinha relacao dual com Epstein**: cientifica (conferencias de virologia) e perturbadora (envio de metodologia de rastreamento de comportamento sexual)

4. **George Church, pioneiro do CRISPR, forneceu a Epstein pesquisa sobre rejuvenescimento** a pedido pessoal e participou de reunioes privadas regulares na residencia de Epstein

5. **Epstein financiou conferencias de biologia sintetica e dinamica viral** com participantes de primeirissimo escalao (Church, Lander, Wolfe, Venter, Nowak)

6. **O interesse de Epstein em eugenia era documentado e conhecido** por cientistas que continuaram a se reunir com ele

7. **O BGC3 trabalhava em "Strain pandemic simulation"** em 2017, e o documento foi encaminhado ao email de Epstein

8. **Nikolic usou a palavra "pandemic"** como area-chave para o DAF em email trilateral com Gates e Epstein em maio de 2017

9. **Epstein usou Rod-Larsen para conectar Gates ao Comite do Nobel da Paz** na Noruega em 2013

10. **O DAF era concebido como "a maior fundacao do mundo"**, atrelado ao programa Gates, com meta de $100 bilhoes em dois anos, envolvendo JPMorgan e Apollo Global

### 13.2 O que e CIRCUNSTANCIAL

1. O "Nathan" mencionado por Gates no cancelamento de dezembro de 2010 pode ser Nathan Wolfe ou Nathan Myhrvold
2. A referencia "girls should be form 5-7 gates from 7-" pode indicar atividades separadas ou apenas logistica de horario
3. A relacao entre o estudo de comportamento sexual proposto por Wolfe e as mulheres de Epstein e sugestiva mas nao documentalmente comprovada
4. A conexao entre a simulacao de pandemia do BGC3 (2017) e a pandemia real (2019-2020) e temporal, nao causal
5. A conexao entre o interesse de Epstein em eugenia e a pesquisa de rejuvenescimento de Church e implicita, nao explicita nos emails

### 13.3 O que NAO TEM BASE nos documentos

1. **Nao ha evidencia de que Epstein financiou pesquisa de criacao de pandemias** ou armas biologicas
2. **Nao ha evidencia de conexao direta** entre Epstein e o laboratorio de Wuhan, gain-of-function, ou EcoHealth Alliance (alem de Nathan Wolfe ter sido membro do conselho da EcoHealth)
3. **Nao ha evidencia de que Gates Foundation** canalizou recursos ilicitos via Epstein
4. **Nao ha evidencia de que as vacinas COVID** estejam conectadas a rede Epstein
5. Os termos Wuhan, Fauci, mRNA, GAVI, CEPI nos documentos sao exclusivamente de artigos de imprensa, nao de comunicacoes de Epstein

### 13.4 O Quadro que Emerge

O que os documentos revelam nao e uma conspiracao pandemica. E algo que, a seu modo, e mais inquietante por ser demonstravel: um traficante sexual condenado posicionou-se no exato ponto de interseccao entre quatro eixos de poder.

**Eixo 1: Riqueza** (Gates, JPMorgan/Staley, Apollo/Leon Black, Dalio, Paul Tudor Jones)
**Eixo 2: Ciencia de fronteira** (Church/CRISPR, Wolfe/pandemias, Venter/genoma, Lander/genomica, Nowak/matematica)
**Eixo 3: Politica e diplomacia** (Comite Nobel, ONU/Rod-Larsen, Larry Summers, Senador Mitchell, Peter Mandelson)
**Eixo 4: Midia e legitimacao** (Michael Wolff, Mort Zuckerman/US News, Reid Hoffman/LinkedIn)

Cada eixo alimentava os demais. Cientistas vinham pelos recursos. Financistas vinham pelas conexoes politicas. Politicos vinham pelo prestigio intelectual. E todos, sem excecao, conferiam a Epstein algo que ele nao podia comprar sozinho: legitimidade.

A pergunta que os documentos deixam em aberto nao e "Epstein criou uma pandemia?" (nao ha base para isso), mas sim: **como e possivel que, apos uma condenacao por crimes sexuais contra menores em 2008, as pessoas mais influentes do mundo em financa, ciencia e politica tenham continuado a jantar na residencia de Epstein por mais de uma decada?**

Os documentos nao respondem essa pergunta. Talvez a resposta seja mais simples, e mais terrivel, do que qualquer conspiracao.

---

## 14. DOCUMENTOS-CHAVE

### 14.1 Relacao Gates-Epstein

| Documento | Data | Conteudo | Relevancia |
|-----------|------|----------|------------|
| EFTA02414311 | 28/11/2010 | "girls should be form 5-7 gates from 7-" | MAXIMA |
| EFTA02410629 | 02/12/2010 | Gates cancela jantar, email de billg@bgc3.com, menciona "Nathan" | ALTA |
| EFTA02320660 | 28/01/2011 | Gates + Nikolic + Peter Mandelson jantar na 71st | MAXIMA |
| EFTA02320685 | 01/02/2011 | Gates + Nikolic duas noites consecutivas | ALTA |
| EFTA02320203 | 02/05/2011 | "Power dinner" Gates + Summers + Staley | MAXIMA |
| EFTA02557253 | Jul/2012 | "Reminder Bill Gates in Norway Aug 6" | MEDIA |
| EFTA02548854 | Jan/2012 | Staley pede "1 on 1 meeting with Bill Gates" via Epstein | ALTA |
| EFTA02565753 | Fev/2013 | Almoco Gates + Senador Mitchell | ALTA |
| EFTA02395031 | 28/01/2014 | Skype Call Gates organizada por Epstein | ALTA |
| EFTA02356983 | 28/01/2014 | Confirmacao Skype Call | ALTA |
| EFTA02395937 | Mar/2014 | Email trilateral Epstein-Gates-Cohen sobre DAF | MAXIMA |
| EFTA02404769 | Mar/2014 | Email trilateral sobre jantar Reid Hoffman | ALTA |
| EFTA00373841 | 14/03/2014 | "TBD Dinner w/Bill Gates" na agenda | ALTA |
| EFTA02587505 | Ago/2014 | Epstein a Thiel: "Bill Gates will be with me" + "head of nobel" | MAXIMA |
| EFTA00363562 | Set/2014 | Agenda Gates: Leon Black, Summers, Zuckerman | ALTA |
| EFTA00363580 | Set/2014 | Agenda Gates: Kathy Ruemmler no Four Seasons | ALTA |
| EFTA02386397 | 25/09/2014 | Gates a Epstein sobre DAF, Ebola, Dalio, Paul Tudor Jones | MAXIMA |
| EFTA02356543 | 05/12/2014 | Staley pergunta se reuniao com Gates esta confirmada | MEDIA |
| EFTA02389903 | 24/05/2017 | Trilateral Gates-Nikolic-Epstein: DAF + "pandemic" | MAXIMA |
| EFTA02342151 | s/d | Michael Wolff: Gates "prodding" reabilitacao de Epstein | ALTA |

### 14.2 Boris Nikolic

| Documento | Data | Conteudo | Relevancia |
|-----------|------|----------|------------|
| EFTA00060795 | Ago/2019 | Testamento: "I appoint BORIS NIKOLIC, as successor Executor" | MAXIMA |
| EFTA00128843 | s/d | FBI CHS report sobre Nikolic como executor | MAXIMA |
| EFTA02421641 | s/d | Nikolic encaminha info sobre Principe Andrew a Epstein | ALTA |
| EFTA02421017 | s/d | "how was your mtg w Nathan?" (Nikolic a Epstein) | ALTA |
| EFTA02377958 | s/d | Nikolic encaminha artigo WSJ "Make Bill Gates Richer" | MEDIA |
| EFTA02571172 | s/d | "awaiting my delayed flight to India where I am meeting Bill" | ALTA |

### 14.3 Nathan Wolfe / Metabiota

| Documento | Data | Conteudo | Relevancia |
|-----------|------|----------|------------|
| EFTA02378487 | s/d | Wolfe envia questionarios de comportamento sexual a Epstein | MAXIMA |
| EFTA02433195 | s/d | Epstein oferece "apt available and a car" a Wolfe | ALTA |
| EFTA02441292 | s/d | Lista participantes conferencia: Wolfe, Church, Lander, Nowak | MAXIMA |

### 14.4 George Church / CRISPR

| Documento | Data | Conteudo | Relevancia |
|-----------|------|----------|------------|
| EFTA00353065 | s/d | "Jeffrey requested the attached pdf" (Rejuvenate) | MAXIMA |
| EFTA00353066 | s/d | PDF Rejuvenate de Church | MAXIMA |
| EFTA00333751 | s/d | "George would gladly meet Jeffrey and Noam Chomsky" | ALTA |
| EFTA00351424 | s/d | Jantar: Martin, George, Joscha, Chomsky no instituto Nowak | ALTA |
| EFTA00329744 | s/d | Church conecta Epstein a Luhan Yang e Geoff Mackay | ALTA |
| EFTA02421924 | s/d | Servico de carro para Church apos visita | MEDIA |

### 14.5 BGC3 / Pandemic Simulation

| Documento | Data | Conteudo | Relevancia |
|-----------|------|----------|------------|
| EFTA02381427 | 03/03/2017 | "Strain pandemic simulation" + neurotechnologies + health info | MAXIMA |

### 14.6 DAF (Donor Advised Fund)

| Documento | Data | Conteudo | Relevancia |
|-----------|------|----------|------------|
| EFTA01300940 | 2013-14 | "largest foundation in the world... 100 billion in 2 years" | MAXIMA |
| EFTA01301114 | s/d | "Project Molecule": Gates & JPMorgan Charitable Giving Fund | MAXIMA |
| EFTA00315353 | s/d | "Why Gates/Apollo" | ALTA |

### 14.7 Terje Rod-Larsen / Nobel

| Documento | Data | Conteudo | Relevancia |
|-----------|------|----------|------------|
| EFTA00020923 | s/d | Investigacao norueguesa: Gates no Comite Nobel via Epstein | MAXIMA |
| EFTA00030938 | s/d | Dagens Naeringsliv: Rod-Larsen-Epstein | ALTA |
| EFTA02499005 | 02/06/2015 | Epstein compartilha artigo Vox sobre Gates e pandemia com Rod-Larsen | ALTA |

### 14.8 Eugenia

| Documento | Data | Conteudo | Relevancia |
|-----------|------|----------|------------|
| EFTA00069900 | s/d | NYT: "seed the human race with his DNA" | MAXIMA |
| EFTA02367335 | s/d | Artigo "Are We Ready for Eugenics?" enviado a Epstein | ALTA |
| EFTA02414772 | s/d | "genius...and eugenics" com Martin Seligman | ALTA |
| EFTA00263107 | s/d | "communicated his fascination with eugenics" | ALTA |

---

## 15. INVESTIGACOES PENDENTES

1. **Identidade do "Nathan" no email de Gates (dez 2010)**: Nathan Wolfe ou Nathan Myhrvold? A resposta determinaria se Gates foi introduzido a Wolfe via Epstein ou se a referencia e a outra pessoa

2. **Conteudo completo do PDF "Rejuvenate" de Church**: O documento foi anexado a email mas nao foi integralmente preservado no corpus. O conteudo cientifico completo esclareceria a extensao da colaboracao Church-Epstein

3. **Detalhes do "Strain pandemic simulation" do BGC3**: O documento EFTA02381427 menciona "deliverables" mas nao inclui as especificacoes tecnicas em si. Quem desenvolveu a simulacao? Quais parametros foram usados?

4. **Relacao Nathan Wolfe e EcoHealth Alliance**: Wolfe foi membro do conselho da EcoHealth. EcoHealth canalizou financiamento do NIH para pesquisa de coronavirus no Wuhan Institute of Virology. A interseccao Wolfe-EcoHealth-Epstein necessita investigacao aprofundada

5. **Destino do DAF/Project Molecule**: O fundo de $100 bilhoes foi implementado? Se sim, sob que nome? Se nao, o que impediu?

6. **Coorte do estudo de comportamento sexual de Wolfe**: Quem seriam os sujeitos do "cohort study" proposto por Wolfe a Epstein? O estudo foi realizado?

7. **Financiamento de Epstein a Nowak alem dos $6.5M publicos**: Houve pagamentos adicionais nao declarados?

8. **Outros participantes das conferencias de biologia sintetica**: As listas de participantes mencionam nomes parciais. Identificacao completa pode revelar conexoes adicionais

9. **Conteudo do "Whitepaper on Neurotechnologies as weapons"**: Este deliverable do BGC3 e potencialmente tao significativo quanto a simulacao de pandemia, mas nao foi investigado

10. **Relacao temporal entre as reunioes Gates-Epstein e o divorcio Gates (2021)**: Melinda Gates citou publicamente as reunioes de Bill com Epstein como fator no divorcio. Os documentos revelam que a relacao era ainda mais profunda do que o admitido publicamente

---

**NOTA FINAL**: Este dossie foi produzido com base exclusivamente em documentos primarios do acervo Epstein (indice Elasticsearch + Neo4j). Nenhuma afirmacao e feita sem documento-fonte verificavel. As conclusoes se limitam ao que a evidencia documental suporta. Onde ha lacunas, as lacunas sao declaradas. Onde ha ambiguidade, a ambiguidade e reconhecida. E onde ha fatos inconvenientes, os fatos falam por si.
