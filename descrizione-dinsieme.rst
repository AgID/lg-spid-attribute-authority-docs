Descrizione d’insieme
=====================


Attributi qualificati
=====================

Un attributo qualificato descrive una proprietà di un’identità. Esso si
definisce qualificato perché è attestato da soggetto cui la legge
conferisce tale potere. Di solito gli attributi qualificati non cambiano
frequentemente nel tempo, e il numero di operazioni in lettura è molto
maggiore di quelle in scrittura; ad esempio, l'attributo associato ad
una patente di guida cambierà alla scadenza del documento, ma nel
frattempo verrà letto numerose volte.

All’interno delle federazioni SPID e CIE possono sussistere diverse
tipologie di attributi qualificati, dipendenti dalla specifica AA che
accede al circuito mediante stipula di una convenzione. La descrizione
di tali attributi è, pertanto, demandata alla specifica AA. Può
accreditarsi come AA, qualunque soggetto che ha il potere di attestare
il possesso e la validità di attributi qualificati in base alle norme
vigenti.

La seguente tabella mostra alcuni esempi di possibili AA e i relativi
attributi qualificati.

+-----------------------+-----------------------+-----------------------+
| Entità                | Attributi             | Esempi di servizi     |
|                       |                       | abilitati             |
+=======================+=======================+=======================+
| ASL /SSN / Fascicolo  | status invalido       | Richiesta permesso    |
| Sanitario             | civile                | ZTL                   |
+-----------------------+-----------------------+-----------------------+
| Catasto               | Immobili intestati;   | Precompilazione campi |
|                       | rendite immobiliari   | per domande (ad es.   |
|                       |                       | TARI)                 |
+-----------------------+-----------------------+-----------------------+
| Gestore delle         | Deleghe e procure     | Attributi             |
| deleghe,              | digitali              | identificativi del    |
| amministrazioni di    |                       | delegante che ha      |
| sostegno e tutele     |                       | creato una delega     |
|                       |                       | digitale: per tutti i |
|                       |                       | servizi di un SP; per |
|                       |                       | una specifica classe  |
|                       |                       | di servizi di un SP;  |
|                       |                       | per una specifica     |
|                       |                       | operazione            |
|                       |                       | appartenente ad una   |
|                       |                       | classe di servizi di  |
|                       |                       | un SP. Informazioni   |
|                       |                       | afferenti la delega.  |
+-----------------------+-----------------------+-----------------------+
| IndicePA\*            | Amministrazione di    | Servizi riservati a   |
|                       | appartenenza; ruolo   | dipendenti pubblici   |
+-----------------------+-----------------------+-----------------------+
| INPS                  | ISEE; status          | Accesso a servizi con |
|                       | pensionistico         | policy basate         |
|                       |                       | sull’ISEE             |
+-----------------------+-----------------------+-----------------------+
| Ministero             | Stato civile;         | Richiesta permesso    |
| dell’Interno (ANPR)   | familiari; luogo di   | ZTL; accesso a        |
|                       | residenza; lista      | servizi               |
|                       | elettorale; titolo di | comunali/regionali    |
|                       | studio e tutti gli    |                       |
|                       | altri campi previsti  |                       |
|                       | dal DPCM 194/2014     |                       |
+-----------------------+-----------------------+-----------------------+
| Motorizzazione        | Classe patente;       |                       |
|                       | neopatentato; saldo   |                       |
|                       | punti patente         |                       |
+-----------------------+-----------------------+-----------------------+
| Notariato\*           | Appartenenza al       | Servizi riservati a   |
|                       | Notariato             | notai                 |
+-----------------------+-----------------------+-----------------------+
| Ordini                | Appartenenza ad un    | Servizi riservati a   |
| professionali\*       | ordine                | professionisti        |
|                       |                       | (concorsi ecc.)       |
+-----------------------+-----------------------+-----------------------+
| Pubblico Registro     | Veicoli intestati     |                       |
| Automobilistico       |                       |                       |
+-----------------------+-----------------------+-----------------------+
| Registro delle        | Imprese di cui il     | Servizi alle imprese; |
| Imprese\* [2]_        | soggetto è socio o    | verifica dei poteri   |
|                       | detiene cariche       | di rappresentanza;    |
|                       |                       | deleghe               |
+-----------------------+-----------------------+-----------------------+
| Registro INI-PEC\*    | PEC                   |                       |
+-----------------------+-----------------------+-----------------------+

.. [1]
   previsti espressamente dal DPCM del 24 ottobre 2014

.. [2]
   previsti espressamente dal DPCM del 24 ottobre 2014


Convenzioni
===========

I Gestori di attributi qualificati (AA) ai sensi dell’articolo 4 lettera
c) del DPCM 26 ottobre 2014, stipulano apposita Convenzione con
l’Agenzia.


Attestazione di attributo
=========================

Le attestazioni di attributo prodotte da un’AA servono ad attestare uno
o più attributi qualificati riguardo ad una persona fisica o giuridica,
previa richiesta da parte di un SP.

Per erogare un servizio, il SP può aver bisogno di una molteplicità di
attributi qualificati attestabili da AA differenti; gli attributi
qualificati attestabili dalla medesima AA sono preferibilmente raccolti
in un’unica richiesta di attributi, a meno che alcuni di questi
attributi siano soggetti a dipendenze verificabili solo previa
attestazione di altri attributi qualificati

Le richieste e le risposte di attributi sono conservate per 24 mesi al
fine di poter ricostruire, in caso di richiesta da parte di un
interessato, il flusso dei dati personali ad esso riferiti. Fatte salve
diverse disposizioni di carattere normativo o amministrativo, è fatto
divieto alle AA e ai SP di conservare tali informazioni per un periodo
di tempo superiore, nonché di trattare le predette informazioni per
finalità diverse da quelle sopraindicate.

È fatto altresì divieto alle AA e ai SP di trattare ogni altro dato
personale di cui siano venuti a conoscenza o a cui abbiano avuto accesso
per le finalità indicate o in attuazione delle presenti linee guida, per
finalità ultronee a quelle indicate nelle stesse.


Tipologie di richiesta
======================

Le singole AA definiscono nelle proprie specifiche OAS3, conformi alle
indicazioni delle LL.GG. Interoperabilità, emanate da Agid, quali siano
gli elementi obbligatori che i SP devono inserire nelle richieste. Fermo
restando l’uso esclusivo delle specifiche OAS3, esclusivamente per la AA
che gestisce le deleghe, amministrazioni di sostegno e tutele, può, in
prima istanza, essere utilizzata l’interfaccia SAML come normato nello
specifico allegato delle presenti LG.

Ogni richiesta di attributi qualificati si caratterizza per:

a) identificazione del soggetto;

b) sincronicità della richiesta di attributi qualificati: puntuale o
   continuativa;

c) verifica della necessità di rilascio del consenso da parte
   dell’utente alla fornitura di attributi qualificati.

Le interrogazioni alle AA sono caratterizzate dalla tipologia dei dati
richiesti, da cui discende l’obbligatorietà da parte delle AA di
acquisire o meno il consenso dell’interessato alla comunicazione dei
propri dati al richiedente (punto a). Per ottenere tale consenso può
essere necessario che la stessa AA acquisisca il consenso
dall’interessato. In altri casi, invece, è possibile che l’AA preveda
che il consenso sia raccolto dal SP.

I SP possono richiedere dati personali nei casi previsti dalla norma con
particolare riferimento al GDPR e al codice privacy.

Qualunque sia la tipologia di identificazione, l’AA decide se (punto c):

-  gli attributi qualificati possono essere inviati al SP previo
   consenso acquisito dal SP o in assenza dello stesso consenso

-  è necessario richiedere all’ utente il consenso esplicito per l’invio
   dei dati al SP.

É prevista (punto b), la possibilità per il SP di richiedere gli
attributi qualificati una tantum (richieste puntuali), o di effettuare
più richieste dei medesimi attributi in automatico nell’arco di un
periodo di lunga durata (richieste continuative).


**Richieste puntuali**

La richiesta di attributi qualificati è puntuale quando, se accolta,
viene seguita da un’unica immediatamente “sincrona” risposta di
attributi da parte dell’AA.


**Richieste continuative**

Le AA possono prevedere richieste continuative.

La richiesta di attributi qualificati è continuativa quando, se accolta,
un SP indirizza ad una AA, relativamente agli stessi attributi
qualificati iniziali, molteplici richieste “asincrone” di attributi,
all’interno di una finestra temporale reciprocamente concordata tra SP,
AA e utente. Tale finestra temporale non potrà in nessun caso essere
superiore ad un periodo ininterrotto di 12 mesi.

La richiesta continuativa è costituita da un consenso di lunga durata,
inizialmente proposto dal SP all’AA che, qualora il consenso sia
accordato, valuta se ammetterne la continuità o meno. L’AA può ritenere
la durata eccessiva e, nel caso, ridurre la finestra temporale a un
periodo inferiore rispetto a quanto proposto dal SP.

Nel caso in cui il consenso di lunga durata sia ammissibile da parte
dell’AA, quest’ultima richiede all’utente di accettare esplicitamente la
finestra temporale, eventualmente abbreviata dall’AA. L’utente può
decidere se:

a) negare tale richiesta continuativa (e quindi negare il consenso a
   fornire gli attributi qualificati in oggetto),

b) convertire la richiesta in una richiesta puntuale, oppure

c) ridurre ulteriormente la durata della finestra temporale a un
   qualunque periodo inferiore di propria scelta.

Una volta acquisito il consenso, il SP può inviare all’AA delle
richieste asincrone limitatamente agli attributi per cui è stata
autorizzata la trasmissione, durante il periodo concordato, senza che
intervenga alcun ulteriore processo di autenticazione o autorizzazione
da parte dell’utente.

All’approssimarsi della scadenza del periodo concordato l’AA può
informare l’utente dell’opportunità di rinnovare o estendere tale
periodo per ulteriori 12 mesi privi di interruzioni .

Il consenso di lunga durata può avere profonde implicazioni in merito
alla minimizzazione dei dati personali. Per tale motivo è sempre
richiesto nel rispetto di quanto previsto dai considerando 71, 78 e 156
e dall’articolo 5, comma 1,lett. c) del Regolamento GDPR.

