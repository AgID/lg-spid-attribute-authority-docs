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

Richieste puntuali
------------------

La richiesta di attributi qualificati è puntuale quando, se accolta,
viene seguita da un’unica immediatamente “sincrona” risposta di
attributi da parte dell’AA.

Richieste continuative
----------------------

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
