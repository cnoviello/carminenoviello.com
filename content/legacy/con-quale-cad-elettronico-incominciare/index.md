+++
title = "Con quale CAD elettronico incominciare?"
slug = "con-quale-cad-elettronico-incominciare"
url = "/2013/08/02/con-quale-cad-elettronico-incominciare/"
date = "2013-08-02T05:58:57Z"
lastmod = "2013-08-02T07:16:57Z"
draft = false
description = "Proprio qualche giorno fa rispondevo a questa domanda di un mio amico che ha da poco ultimato il suo primo progetto con Arduino. Ha realizzato tutto su breadboard e dopo…"
categories = ["Others"]
tags = ["altium","Arduino","cad elettronico","eagle","incominciare elettronica","orcad","pulsonix"]
showHero = true
showTableOfContents = true

[cover]
image = "images/legacy/con-quale-cad-elettronico-incominciare/cover-schermata-2013-07-31-alle-05-56-43.png"
alt = "Schermata 2013-07-31 alle 05.56.43"
hiddenInSingle = false
+++

Proprio qualche giorno fa rispondevo a questa domanda di un mio amico che ha da poco ultimato il suo primo progetto con Arduino. Ha realizzato tutto su breadboard e dopo tentativi, aggiustamenti e cambi, ha praticamente "finalizzato" la sua progettazione. A me piace chiamarlo *design by attempt* e, se siete interessati a seguire un percorso nell'elettronica, scoprirete che anche per progetti molto complessi si finisce sempre a fare qualche tentativo: a volte, prima di chiudere un prodotto se ne passano 3-4 sbrogli prima di poter mettere la parola fine. Forse.

Quando si passa dalla breadboard alla progettazione vera e propria serve ovviamente uno strumento che aiuti in questo percorso: un CAD è per l'appunto uno strumento di ausilio allo sviluppo di un progetto, e un CAD elettronico ha tutte le feature necessarie per fare progettazione elettronica. Tuttavia, immergersi in un CAD elettronico è un'esperienza lunga, faticosa e costellata di errori. Rassegnatevi all'idea che i primi progetti avranno più problemi per non conoscere lo strumento in sé che per aver commesso errori relativi al progetto in quanto tale. Spesso, basta un nome sbagliato di una *net *per ritrovarsi con un errore sul circuito stampato finale (una *net* è un ramo di connessione tra due parti di un circuito, e ricordate queste parole: una *net list* ordinata è la differenza tra una progettazione andata a buon fine e una disastrosa).

Già: ma con quale CAD elettronico cominciare? Se siete giunti a questo articolo probabilmente siete alle ricerca di un prodotto. Forse vi siete già fatti un'idea, forse avete già letto tante cose in giro, forse vi frullano per la testa delle sigle. Lungi da me entrare in una delle solite guerre di religione che spesso tormentano il web tra cosa è meglio di cosa. Però posso dire con estrema sicurezza che ci sono due punti che dovete evitare nella maniera più assoluta durante questa scelta:

1.  Evitare di dedicare tempo e risorse (magari anche economiche) a CAD che a stento superano la dimensione di prodotto hobbistico. Dispiace dirlo. E fa male sentirlo dire soprattutto da un informatico che sa perfettamente che tutti i grandi prodotti sono nati a partire da due componenti fondamentali: la passione e la dedizione. Tuttavia, voi volete fare le cose sul serio. E il fatto che quello strumento sia dato gratis, o che per qualche strano motivo sia preso a cuore da una community a punto da eleggerlo "strumento indispensabile", non significa che fa per voi a tutti i costi. Per imparare ad usare un CAD occorrono anni, ed un CAD deve fornire degli strumenti minimali per fare buona progettazione elettronica. Due su tutti: uno strumento di ERC e di DRC. Il primo è acronimo di *Electrical Rule Checking*, ed è uno strumento di verifica formale che vi permette di valutare la presenza di grossolani errori di progettazione nel disegno del circuito (badate bene: non vi dirà mai che quel circuito è sbagliato, vi dice solo che avete violato delle regole minimali; la semantica del progetto è altra cosa - Sic!). Il secondo è acronimo di *Design Rule Checking* ed è uno strumento di verifica fondamentale per la fase di sbroglio del circuito (un DRC configurato bene è TUTTO), che vi segnala eventuali sovrapposizioni di rami di connessione, violazione delle regole di produzione, ecc,ecc. Quindi, lasciate stare prodotti troppo semplici: voi volete fare le cose sul serio, e vi occorre un prodotto serio.
2.  L'ultima frase del punto di cui sopra genera un altro errore da evitare come la peste: lasciate stare CAD mastodontici, blasonati e ultra complessi. Altium, Orcad, Allegro, Pulsonix sono solo i nomi dei più famosi e complessi CAD che troverete in giro. Se già avete visitato i loro siti web super-sexy, pieni di video incredibili, immagini mozzafiato che vi faranno sentire il più evoluto progettista elettronico del mondo, sappiate che siete caduti nella sindrome che io chiamo "*solo il meglio per fallire*". È una sindrome molto diffusa ai giorni nostri tra chi ha una passione di qualunque tipo. Voglio comprare la moto? Solo quella da €30.000! Voglio una bici? Solo quella da €3000. Voglio un CAD elettronico? Solo quello da €10.000 a licenza, con miliardi di strumenti che non userò mai - ma non si sa mai nel caso.\
    Sbagliato. Reset your head! Se state leggendo questo articolo, voi di progettazione elettronica non ne sapete niente. E se partite da uno di quei programmi o fallirete miseramente, o abbandonate dopo 2-3 giorni. Occorrono mesi di duro lavoro per capire i meccanismi di base della progettazione e, soprattutto, della realizzazione del PCB. Avrete bisogno di fare delle cose e fare degli errori. Ma c'è una cosa di cui non avete proprio bisogno: che lo strumento di aiuto vi si ritorca contro. Non sto dicendo che magari un giorno non finirete la. E ci sono decine di ottimi motivi per usare uno di questi strumenti. Ma non è il momento. Le ossa prima di tutto.

\
A questo punto il campo si è maledettamente ristretto a qualche nome. Esistono dei CAD di media dimensione. Che io sappia, esistono delle costole di Pulsonix nate per il settore educational. Tuttavia, quasi sicuramente se sulla vostra scrivania c'è un Arduino allora avrete sentito parlare di [Eagle](http://www.cadsoftusa.com/).

Eagle è un CAD elettronico di medie dimensioni. Recentemente l'azienda che lo produce è stata acquisita da Premier Farnell, ed è un prodotto destinato ad evolvere nel futuro. Ha dalla sua molti vantaggi, tra cui:

- Multipiattaforma: è l'unico CAD degno di questo nome che gira perfettamente su Windows, Linux e Mac OS. Non è poco.
- Intuitivo: ha una curva di apprendimento dolce e non traumatica. Sicuramente ciò che vi serve per cominciare.
- È supportato dalla community: a causa delle sua licenza (ne parlo tra poco), intorno ad Eagle si sono sviluppati decine di progetti di ULP e librerie free che lo rendono molto completo. A volte si trovano cose per Eagle che i CAD blasonati non hanno. Non è poco.
- Arduino oriented: è il CAD con cui progettano e sbrogliano Arduino. E ci troverete tutto quello che ronza intorno a questa piattaforma. Compresi i progetti dei vari Sparkfun, Adafruit, ecc.
- Ha una licenza freeware: a patto di accettare alcune limitazioni, Eagle ha una licenza freeware che permette di adoperarlo senza acquistare una licenza. La vostra coscienza digitale vi ringrazierà.
- Ha un prezzo abbordabile: ok, vi siete evoluti. Oggi avete fatto della vostra passione un mestiere. Avete bisogno di una licenza PRO di Eagle. La buona notizia e che non vi occorre un leasing. E non ci sono licenze annuali da rinnovare. Di questi tempi non è poco.

I piani di licenza di Eagle sono il motivo che hanno permesso la diffusione di questo CAD nelle community Open Hardware. La licenza freeware vi permette di [scaricare gratuitamente](http://www.cadsoftusa.com/download-eagle/) l'ultima versione di Eagle (la 6.4 al momento) a [queste condizioni](http://www.cadsoftusa.com/download-eagle/freeware/?language=en):

- Possono essere adoperati al massimo d 2 layer di segnali (e credete a me: sbrogli con più di 2 layer costano e vanno fatti quando c'è ne è realmente bisogno).
- La dimensione massima del PCB è di 100x80 mm.
- L'editor dello schema vi consente di avere un solo foglio (a dirla tutta la gestione degli sheet in Eagle non è sta grande cosa, almeno fino a Eagle 5.x).
- Potete adoperare il programma solo per realizzare progetti senza fini di lucro, ossia per hobby o per rilasciarli alla comunità in Open Hardware.

Insomma, c'è tutto per cominciare. L'unica cosa che manca in realtà è l'autorouter. Tuttavia, ascoltate un consiglio: oltre al fatto che l'autorouter di Eagle fa solo danni, se volete imparare qualcosa dimenticate questa parola! Se la limitazione sul numero di layer di segnali e sulla dimensione della scheda è troppo restrittiva per voi, allora potete acquistare una licenza [Hobbyst](http://www.cadsoftusa.com/shop/eagle-hobbyist-and-education/) che al prezzo di circa €140,00 vi permette di realizzare schede di 100x160 mm, con 6 layer di segnali. Unica limitazione è che i progetti non possono essere usati per fini commerciali (in sostanza non ci potete guadagnare dal progetto realizzato).

Eagle ha tutto (e molto di più) quello che serve per cominciare. Un buon gestore del progetto (schematic editor) e un discreto editor di layout, che vi permetterà di realizzare lo sbroglio. Poi su Eagle si trovano in giro decine di tutorial e anche molti video su Youtube. Cercando su google troverete ogni risposta a qualsiasi domanda. Nella sezione [download](http://www.cadsoftusa.com/download-eagle) del sito ufficiale di Eagle troverete molte altre librerie da scaricare, ULP (acronimo di *User Language Program*, ossia il linguaggio di Eagle che permette di sviluppare script di automazione), utility e documentazione varia.

È chiaro che,come ogni cosa, Eagle ha i suoi difetti e limiti. Tuttavia, io vi dico di trovarli da voi. Lasciate stare quello che si dice in giro. Se il difetto non lo trovate, allora non è critico per il vostro ciclo di lavoro. E comunque ripeto: fino a che non avrete la necessità di realizzare progetti molto complessi, Eagle ha tutto quello che serve.

Tornerò a parlare di Eagle nel prossimo futuro, soprattutto per aspetti legati alla produzione dei circuiti. A presto.
