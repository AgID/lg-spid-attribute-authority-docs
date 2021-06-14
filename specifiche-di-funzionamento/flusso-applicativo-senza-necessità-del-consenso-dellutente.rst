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

.. |image0| image:: /media/image2.png
   :alt:Figura 1 Flusso di richiesta di attributi qualificati senza consenso o consenso acquisito dal SP.
   :width: 6.21528in
   :height: 4.04861in
