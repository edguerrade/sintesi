Requeriments
============

Es vol desenvolupar un sistema de gestió de faltes d'assistència de l'alumnat d'un centre educatiu com ara l'IES Joan d'Àustria.

Els usuaris de l'aplicació seran el tutor i els docents que formen l'equip docent dels diferents grups d'alumnes. A més hi haurà un administrador (probablement el cap de departament) que, podria ser a l'hora tutor i docent.

L'aplicació ha de ser accessible des de un ordinador amb connexió web i un navegador estàndard (MS Explorer, Firefox i Chrome en versions actuals a l'inici del desenvolupament)

El programa acceptarà una càrrega massiva des d'un fitxer csv (per definir el format) però també l'administració interactiva d'aquells elements nombrosos com ara llistats d'alumnes, cursos, docents, etc.

De la mateixa manera, també es podrà extreure aquesta informació en csv.

En començar l'any acadèmic, l'administrador:

1.	crea un nou any acadèmic al sistema

2.	gestiona els cursos, les unitats d'impartició o classes, i els subgrups.

	Els cursos són agrupacions de classes. Per exemple, DAI, DAW, ASIX, SMX.

	Els cursos tenen un nom (ex. Desenvolupament d'Aplicacions Web) i un acrònim (ex. DAW)

	Les classes són la únitat mínima en la que un alumne pot estar matriculat. Per exemple, M01UF1, M01UF2, M12, etc.

	De les classes en voldrem saber el nom (ex. Instal·lació, configuració i explotació del sistema informàtic), un codi (ex. M01UF1), i la durada oficial en hores.

	De la majoria de classes només hi haurà un grup d'alumnes. Hi ha, però, classes molt nombroses que es divideixen en subgrups. Dels subgrups voldrem saber un nom (ex. A o matí) i la distribució d'hores setmanal (ex. dilluns i dijous 2 hores, divendres 1 hora)

	Totes aquestes dades es mantenen força estables al llarg dels anys acadèmics, però de vegades hi ha canvis importants (es modifica un curs, es substitueix un curs per un altre però han de conviure tots dos durant un temps) Per aquesta raó, cal disposar d'una càrrega massiva d'aquestes dades però no d'un manteniment interactiu.

	L'administrador, normalment, introduirà a l'aplicació el fitxer extret de l'aplicació el curs anterior. El primer cop, és clar, se l'haurà de preparar pel seu compte.

3.	gestiona els docents.

	Dels docents únicament introdueix la part del nom de l'adreça de correu electrònic del centre. Per exemple, *ana.riu* de l'adreça *ana.riu@iesjoandaustria.org*. No es preveu que hi hagi docents sense correu corporatiu. Amb tot, el domini del correu s'ha de poder configurar.

4.	gestiona l'assignació subgrup-classe/docent

	Cada subgrup, o classe d'un sol grup, ha de tenir un docent assignat. Els subgrups/classes sense docent assignat, apareixeran ressaltades als llistats mentre no se'ls assigni un.

	Els docents poden anar canviant al llarg del curs (ex. substitucions) Per aquesta raó, l'aplicació permetrà realitzar amb agilitat canvis d'assignació i indicar períodes en els que el docent està assignat. Ex. un docent pot estar assignat tot el curs, però del 27/2 al 31/4 un altre docent també estarà assignat perquè el substitueix.

	Evidentment, un mateix docent pot estar assignat a un o més subgrups d'una classe. En aquest cas, probablement els horaris dels subgrups no coincidiran. Però aquesta comprovació queda fora dels objectius de l'aplicació a desenvolupar.

5.	introdueix les tutories i els tutors assignats

	Les tutories corresponen als cursos no a les classes. Normalment hi ha una tutoria pel primer any d'un curs i una pel segon any. Per fer-ho general, l'administrador determinarà el nombre de tutories i li posarà un nom (ex. DAW1 per primer de DAW)

	Els alumnes d'un curs estan associats a una tutoria o a una altra, amb independència de les classes en les que estiguin matriculats. Per exemple, un alumne pot ser de segon però tenir alguna classe pendent de primer.

	Cada tutoria ha de tenir, com a mínim, un tutor. Si a un curs no se li ha assignat cap tutor a alguna de les tutories creades, es mostrarà ressaltat.

	Els alumnes corresponents a una tutoria seran assignats al primer tutor introduït. De la mateixa manera, tots els alumnes seran inicialment assignats al primer subgrup de cada classe. Aquestes assignacions podran ser canviades per qualsevol dels tutors assignats en qualsevol moment.

	Quan hi ha més d'un tutor per un curs, normalment hi ha més d'un subgrup a una o més classes. Els tutors aniran autoassignant-se els alumnes i distribuint-los entre els subgrups. L'assignació d'alumnes a un tutor té com a objectiu que el tutor pugi decidir veure només els alumnes que té assignat. En tot cas sempre podrà, si vol, realitzar qualsevol acció disponible amb tots els alumnes de la tutoria.

Un cop creat l'estructura de l'any acadèmic, qualsevol dels tutors assignats a una tutoria se n'encarrega d'introduir:

1.	els alumnes matriculats a la seva tutoria: nom, cognoms, dni, email, telèfon

	Algunes d'aquestes dades poden ser desconegudes pel tutor. L'aplicació permetrà introduir alumnes sense les dades de contacte o el DNI, però els mostrarà ressaltats als llistats del tutor fins que disposin de totes les dades.

2.	els cursos realitzats per cada alumne

	Un alumne pot estar matriculat a un curs per primer cop, o bé repetint-lo.

Un cop començat el curs acadèmic, cada docent podrà accedir a l'aplicació per indicar el nombre d'hores que ha faltat cada alumne a les classes que imparteix.

Per fer-ho, el docent seleccionarà la classe/subgrup de la llista de classes que té assignades, la data (per defecte l'actual i només seran vàlides les dates de la setmana que s'imparteix la classe) i marcarà el nombre d'hores que cada alumne falta a la sessió d'aquell dia. L'aplicació controlarà que no es pugui marcar més hores de les que té assignades la classe per a aquell dia de la setmana.

Al docent només li apareixeran els alumnes que tingui assignats cada moment pel subgrup o la classe seleccionada. Pot passar, però, que vulgui introduir dades de faltes d'un alumne de la classe que ha estat canviat a un altre subgrup al que el docent no estigui assignat. Per donar resposta a aquesta casuística (i d'altres similars), el docent podrà marcar alguna opció que li permeti veure la resta d'alumnes de la classe i gestionar les faltes.

També podrà indicar un retard en comptes del nombre d'hores faltades.

En cas que ho trobi oportú, el docent podrà afegir un comentari per dia. Per exemple, "avui hi ha vaga de transports i per això molts alumnes arriben tard"

Els docents també podran descarregar-se la llista dels seus alumnes i pujar les faltes d'assistència en format csv.  D'aquesta manera els docents podran passar llista amb alguna eina local (ex. un full de càlcul) i quan tinguin connexió, pujar el fitxer amb les faltes.

Cal tenir en compte que el tutor d'un grup d'alumnes pot ser també docent del grup, i de fet, sol ser-ho.

Quan el docent ha assignat les faltes d'un dia determinat les podrà modificar (afegir o treure faltes) però l'aplicació marcarà el canvi com una correcció i guardarà la data de realització i el valor anterior (per cada correcció que es realitzi). El docent podrà deixar un comentari per explicar el canvi.

Els tutors també hauran de passar llista a les sessions de tutoria.

Si bé és desitjable que l'aplicació ofereixi agilitat en l'ús de totes les opcions, en el cas de l'ús del docent és especialment crític, donat que sovint han de fer la seva tasca en un temps molt reduït durant la classe.

Quan els alumnes porten un justificant vàlid, el tutor pot marcar com a justificades una o més faltes.

Els tutors podran disposar d'informes de faltes en qualsevol moment. Aquests informes inclouran, com a mínim, les següents possibilitats

+ alumnes: per un alumne concret, per tots els alumnes assignats al tutor, per tots els alumnes	assignats a la tutoria, alumnes amb un nombre de faltes superior a un cert percentatge a indicar.

+ classes/subgrups: per una classe concreta, un subgrup concret, tots els subgrups d'una classe, totes les classes del curs.

+ informació: nombre de faltes, nombre de retards, nombre de faltes justificades, nombre de faltes no justificades, total d'hores no justificades comptant la penalització per retards (un valor de	configuració indicarà quants retards equivalen a una falta), comentaris, docents que han posat la falta, correccions de faltes.

Aquests informes es podran exportar a csv.

Com a ampliació, es proposa oferir la possibilitat de mantenir informació històrica dels cursos, i de duplicar l'estructura d'aquests (ex. docents, classes/subgrups, etc.)
