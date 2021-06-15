Sigle e Riferimenti
===================


Riferimenti Normativi
---------------------

Sono riportati di seguito gli atti normativi di riferimento del presente
documento.

-  **[D.Lgs. 82/2005]** Decreto legislativo 7 marzo 2005, n. 82 recante
   “Codice dell’amministrazione digitale”; NOTA – Il D. Lgs. 82/2010 è
   noto anche con l’abbreviazione “CAD”


Standard di riferimento
-----------------------

Sono riportati di seguito gli standard tecnici di riferimento per
l’applicazione del presente documento.

-  **[OAS v3]** Open API Specification v3

-  **[RFC-7515]** JSON Web Signature (JWS)

-  **[SAMLcore]** Security Assertion Markup Language (SAML) v2.0


Linee guida di riferimento
--------------------------

Di seguito sono elencate le Linee Guida e le Regole Tecniche emesse
dall’AGID che verranno richiamate nel presente documento:

-  Linea di indirizzo sulla interoperabilità tecnica (Determinazione
   AgID n. 406/2020);

-  Linee guida contenenti Regole tecniche relative all’uso di OpenID®
   Connect nella federazione SPID;

-  Linee guida contenenti Regole tecniche circa la sottoscrizione
   elettronica di documenti mediante SPID ex art. 20 del CAD.


Termini e definizioni
---------------------

Ai fini delle presenti Linee guida, oltre ad applicarsi le definizioni
di cui all’articolo 1 del CAD, si intende per:

-  **Attestazione di attributo/i** : cfr. ‘risposta di attributi’;

-  **Attributi qualificati** : le qualifiche, le abilitazioni
   professionali e i poteri di rappresentanza e qualsiasi altro tipo di
   attributo attestato da un gestore di attributi qualificati, ivi
   compresi i dati relativi al possesso di abilitazioni o autorizzazioni
   richieste dalla legge ovvero stati, qualita' personali e fatti
   contenuti in albi, elenchi o registri pubblici o comunque accertati
   da soggetti titolari di funzioni pubbliche, secondo le modalita'
   stabilite da AgID con Linee guida.

-  **Gestori di attributi qualificati**: i soggetti accreditati ai sensi
   dell'art. 16 del DPCM 24 0ttobre 2014 che hanno il potere di
   attestare il possesso e la validità di attributi qualificati, su
   richiesta dei fornitori di servizi;

-  **Registro SPID** : elenco dei soggetti appartenenti alla federazione
   SPID, disponibile su internet all’indirizzo
   https://registry.spid.gov.it che pubblica, per ciascuno di essi, le
   informazioni pubbliche di pertinenza per lo schema, come ad esempio
   il codice IPA e il campo entityId;

-  **Regolamento eIDAS** : Regolamento (UE) N°910/2014 del Parlamento
   Europeo e del Consiglio, del 23 luglio 2014, in materia di
   identificazione elettronica e servizi fiduciari per le transazioni
   elettroniche nel mercato interno e che abroga la direttiva
   1999/93/CE;

-  **Regolamento GDPR** : Regolamento (UE) N°679/2016 del Parlamento
   Europeo e del Consiglio, del 27 aprile 2016, relativo alla protezione
   delle persone fisiche con riguardo al trattamento dei dati personali,
   nonché alla libera circolazione di tali dati e che abroga la
   direttiva 95/46/CE;

-  **Richiesta di autenticazione** : l’evidenza informatica con la quale
   un SP richiede l’avvio di una sessione di autenticazione presso un
   IDP (cioè l’authentication request nei contesti SAML e OIDC);

-  **Richiesta di attributi** : l’evidenza informatica con la quale un
   SP richiede a un’AA uno o più attributi qualificati di un soggetto;

-  **Risposta di autenticazione** : l’evidenza informatica con la quale
   un IDP comunica i dati personali, o il diniego a fornirli, presso un
   SP (response nel contesto SAML; user-info o id token nel contesto
   OIDC);

-  **Risposta di attributi** : l’evidenza informatica con la quale un’AA
   comunica a un SP uno o più attributi qualificati (cd. attestazione di
   attributo), ovvero il diniego a fornirli;


Acronimi e abbreviazioni
------------------------

Di seguito si riportano gli acronimi e le abbreviazioni che verranno
utilizzati nella presente Linee Guida:

-  **Agenzia** o **AgID :** Agenzia per l’Italia Digitale;

-  **PA** : Pubblica Amministrazione;

-  **AA** : attribute authority (gestori di attributi qualificati);

-  **CA** : certificate authority;

-  **CAD** : D.Lgs. 7 marzo 2005 N°82, Codice dell’Amministrazione
   Digitale, e s.m.i.

-  **OIDC** : OpenID Connect;

-  **OAS3** : OpenAPI Specification (OAS), versione 3.0;

-  **CF** : codice fiscale;

-  **CIE** : Carta di Identità Elettronica;

-  **IDP** : identity provider;

-  **JSON** : JavaScript Object Notation, come previsto dalla norma
   RFC-8259;

-  **JWT** : pacchetto JSON (JSON Web Token), come previsto dalla norma
   RFC-7797;

-  **JWE** : JWT cifrato, come previsto dalla norma RFC-7516;

-  **JWS** : JWT firmato, come previsto dalla norma RFC-7515;

-  **OAS3** : si veda OpenAPI;

-  **OIDC** : standard OpenID Connect pubblicato da OpenID® Foundation;

-  **IPA** : indice degli indirizzi della pubblica amministrazione;

-  **PKI** : Public Key Infrastructure (infrastruttura a chiave
   pubblica), basata su certificati elettronici conformi a RFC-5280;

-  **QTSP** : prestatore di servizi fiduciari qualificati ai sensi del
   regolamento eIDAS;

-  **QSEAL** : sigillo elettronico avanzato, come da regolamento eIDAS;

-  **SAML** : standard Security Assertion Markup Language, versione 2.0,
   pubblicato da OASIS;

-  **SP** : fornitore di servizi nella federazione SPID, ovvero service
   provider nel contesto SAML, ovvero relying party nel contesto OIDC;

-  **SPID** : Sistema Pubblico di Identità Digitale, introdotto con il
   DPCM del 24 ottobre 2014, articolo 4, comma 2 e successive
   modificazioni;


Basi giuridiche
---------------

L’articolo 1, comma 1, lett. m), decreto del Presidente del Consiglio
dei ministri 24 ottobre 2014 definisce i gestori di attributi
qualificati (AA) come:

[…] i soggetti accreditati ai sensi dell’articolo 16 che hanno il
potere, in base alle norme vigenti, di attestare il possesso e la
validità di attributi qualificati, su richiesta dei fornitori di
servizi.

Tali attributi qualificati sono definiti, all’articolo 1, comma 1, lett.
e), decreto del Presidente del Consiglio dei ministri 24 ottobre 2014,
come:

[…] le qualifiche, le abilitazioni professionali e i poteri di
rappresentanza e qualsiasi altro tipo di attributo attestato da un
gestore di attributi qualificati.

L’articolo 16, comma 3, prevede che:

Su richiesta degli interessati, sono accreditati di diritto i seguenti
gestori di attributi qualificati:

a) il Ministero dello Sviluppo Economico in relazione ai dati contenuti
nell’indice nazionale degli indirizzi PEC delle imprese e dei
professionisti di cui all’articolo 6-bis del CAD;

b) i consigli, gli ordini e i collegi delle professioni regolamentate
relativamente all’attestazione dell’iscrizione agli albi professionali;

c) le camere di commercio, industria, artigianato e agricoltura per
l’attestazione delle cariche e degli incarichi societari iscritti nel
registro delle imprese;

d) l’Agenzia in relazione ai dati contenuti nell’indice degli indirizzi
della pubblica amministrazione (IPA) e dei gestori di pubblici servizi
di cui all’articolo 6-ter del CAD.

L’articolo 64 del CAD, come modificato dal decreto semplificazioni,
garantisce il diritto dei cittadini di accedere ai servizi online con lo
SPID e con la CIE. Pertanto, la fruizione dei servizi derivanti dalle
seguenti linee guida devono essere garantiti anche ai cittadini che
utlizzano la CIE (in seguito, federazione CIE) per l’accesso ai servizi
in rete.


.. forum_italia::
   :topic_id: 24570
   :scope: document
