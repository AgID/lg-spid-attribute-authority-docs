Flusso applicativo senza necessità del consenso dell’utente
===========================================================

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

   16. .. rubric:: Flusso applicativo che richiede il consenso
          dell’utente
          :name: flusso-applicativo-che-richiede-il-consenso-dellutente

|image1|

Figura 2 Flusso di richiesta di attributi qualificati con consenso

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

   17. .. rubric:: Infrastruttura a chiave pubblica (pki) e trust model
          :name: infrastruttura-a-chiave-pubblica-pki-e-trust-model

È istituita presso AgID un’infrastruttura a chiave pubblica (PKI)
gerarchica, mediante una CA radice (root CA). Tramite detto sistema di
fiducia AA e SP possono verificare la firma dei messaggi scambiati con
la controparte.

.. |image0| image:: ./media/image2.png
   :width: 6.21528in
   :height: 4.04861in
.. |image1| image:: ./media/image3.png
   :width: 6.23958in
   :height: 4.15625in
