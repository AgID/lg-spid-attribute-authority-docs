Specifiche di funzionamento 
============================


Flusso applicativo senza necessità del consenso dell’utente
-----------------------------------------------------------

Tale flusso si applica anche nel caso in cui il consenso dell’utente sia
già stato acquisito dal SP.

|image0|

Figura 1 Flusso di richiesta di attributi qualificati senza consenso o
consenso acquisito dal SP.

Nel caso di richiesta “sincrona” (cfr. Figura 1):

1. L’utente chiede l’accesso ad un servizio del SP e seleziona l’IdP
   presso il quale ha l’identità digitale.

2. l SP invia una richiesta di autenticazione presso l’IdP di cui al
   punto 1.

3. L’IdP esegue la procedura di autenticazione e invia la risposta di
   autenticazione al SP.

4. Il SP richiede all’AA, informando l'utente in base alla normativa
   Privacy, gli attributi qualificati dei quali ha bisogno;

5. L’AA risponde direttamente al SP fornendo gli attributi richiesti.

.. |image0| image:: ../media/image2.png
   :alt: Figura 1 Flusso di richiesta di attributi qualificati senza consenso o consenso acquisito dal SP.
   :width: 6.21528in
   :height: 4.04861in


Flusso applicativo che richiede il consenso dell’utente
-------------------------------------------------------

|image0|

Figura 2 Flusso di richiesta di attributi qualificati con consenso.

Nel caso di richieste “sincrona” e “asincrona” (cfr. Figura 2):

1. L’utente chiede l’accesso ad un servizio del SP e seleziona l’IDP
   presso il quale ha l’identità digitale.

2. Il SP invia una richiesta di autenticazione presso l’IDP di cui al
   punto 1.

3. L’IDP esegue la procedura di autenticazione e invia la risposta di
   autenticazione al SP.

4. Il SP, avendo bisogno di uno o più attributi qualificati, si avvale
   dell’uso di una AA, informando l’utente secondo quanto previsto dalla
   sulla protezione dei dati personali.

5. L’AA identificata l’utente, ovvero richiede all’utente la prova di
   avvenuta autenticazione dell’utente presso l’IDP.

6. L’AA ottiene prova di avvenuta autenticazione e avvenuto consenso al
   rilascio dei dati presso il SP.

7. L’AA fornisce gli attributi qualificati dell’utente al SP.

Nel processo di autenticazione dell’utente, l’AA può richiedere all’ IDP
l’indirizzo di posta elettronica dell’utente, al fine di inviargli le
seguenti comunicazioni via email:

-  nel caso in cui l’ AA abbia acquisito il consenso di lunga durata,
   dove è disponibile il servizio in rete accessibile tramite SPID per
   gestire (rinnovo o revoca) i consensi di lunga durata;

-  all’ approssimarsi della scadenza del consenso di lunga durata,
   informativa all’ utente dell’ imminente scadenza indicando il
   servizio in rete accessibile tramite SPID per poter eventualmente
   rinnovare il consenso secondo le modalità esposte al §5.3.2.

.. |image0| image:: ../media/image3.png
   :alt: Figura 2 Flusso di richiesta di attributi qualificati con consenso.
   :width: 6.23958in
   :height: 4.15625in


Infrastruttura a chiave pubblica (pki) e trust model
----------------------------------------------------

È istituita presso AgID un’infrastruttura a chiave pubblica (PKI)
gerarchica, mediante una CA radice (root CA). Tramite detto sistema di
fiducia AA e SP possono verificare la firma dei messaggi scambiati con
la controparte.


Servizio di consultazione per l’utente
--------------------------------------

Nel caso in cui sia previsto per norma e nel caso in cui siano
consentite richieste di attributi continuative per mezzo di consenso di
lunga durata, l’utente DEVE disporre di un servizio di consultazione
tramite il quale, accedendovi tramite gli strumenti previsti
dall’articolo 64 del CAD, può prendere visione delle trasmissioni dei
propri dati personali (inclusi gli attributi qualificati) inviati a
soggetti terzi ed esercitare i propri diritti legati al loro
trattamento.

Nel caso in cui, invece, il servizio di consultazione non sia previsto
per norma e l’AA non consenta richieste di attributi continuative,
l’implementazione del servizio di consultazione per l’utente è
facoltativa.

Con particolare riferimento ai consensi di lunga durata, se previsti
dalla AA, accordati all’AA a seguito di richieste di attributi
continuative, l’utente può usare servizi di consultazione per:

-  verificare verso quali SP sono stati accordati tali consensi;

per ciascuno dei consensi di cui al punto precedente:

-  verificare la data, l’ ora e l’ attestazione di attributi inviata per
   ciascuna delle richieste asincrone avvenuta entro il periodo
   concordato per effetto del consenso;

-  accorciare la durata del consenso di lunga durata;

-  revocare il consenso di lunga durata;

Il servizio di consultazione deve essere implementato come API OAS3 ed
essere esposto all’utente tramite applicazione web mobile.


Registro delle Attribute Authority
----------------------------------

L’articolo 16, comma 2, decreto del Presidente del Consiglio dei
ministri 24 ottobre 2014 prevede che “L'Agenzia inserisce in un apposito
registro, accessibile da parte dei fornitori di servizi, le tipologie di
dati resi disponibili da ciascun gestore di attributi qualificati”.

Presso il registro SPID è pubblicato un registro delle AA.

Per le AA basate su OAS3, nel registro SPID è reso disponibile il
relativo documento OpenAPI.

Per la AA che gestisce le deleghe, amministrazioni di sostegno e tutele
è reso disponibile un apposito metadata la cui struttura è pubblicata da
AgID con apposito Avviso.
