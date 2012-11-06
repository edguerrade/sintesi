FUNCIONALITATS
==============

## ABBR

*BREAD = "Browse, Read, Edit, Add, Delete"

*ADMIN = "Usuari Rol Administrador o Cap d'Estudis/Departament"

*TUTOR = "Usuari Rol Tutor"

*DOCENT = "Usuari Rol Docent/Professor"

*FALTA = "S'enten per la falta d'assistencia o la seva variant com a retard"

*RPT = Report / Informe

## USUARIS

Codi: **USERBROWSE**

>Títol: Cercar/Filtrar/Llistar Usuaris

>Actor: ADMIN

>Descripció: Permet cercar, filtrar i llistar els diferents usuaris per nom i cognoms o correu.

Codi: **USERREAD**

>Títol: Mostrar detalls Usuaris

>Actor: ADMIN

>Descripció: Permet veure els detalls i la informació completa de l'usuari desitjat.

Codi: **USEREDIT**

>Títol: Editar Usuaris

>Actor: ADMIN

>Descripció: Permet editar la informació de l'usuari.

Codi: **USERADD**

>Títol: Afegir Usuaris

>Actor: ADMIN

>Descripció: Permet afegir/crear nous usuaris a l'aplicatiu.

Codi: **USERDEL**

>Títol: Eliminar Usuaris

>Actor: ADMIN

>Descripció: Permet eliminar/esborrar usuaris de l'aplicatiu.

## ALUMNES

Codi: **ALUMNEBROWSE**

>Títol: Cercar/Filtrar/Llistar Alumnes

>Actor: ADMIN, TUTOR, DOCENT

>Descripció: Permet cercar, filtrar i llistar els diferents alumnes per nom, cognoms o dni.

Codi: **ALUMNEREAD**

>Títol: Mostrar detalls Alumnes

>Actor: ADMIN, TUTOR, DOCENT

>Descripció: Permet veure els detalls i la informació completa de l'alumne desitjat.

Codi: **ALUMNEEDIT**

>Títol: Editar Alumnes

>Actor: ADMIN, TUTOR

>Descripció: Permet editar la informació de l'alumne.

Codi: **ALUMNEADD**

>Títol: Afegir Alumnes

>Actor: ADMIN, TUTOR

>Descripció: Permet creat/afegir nous alumnes a l'aplicatiu.

Codi: **ALUMNEDEL**

>Títol: Eliminar Alumnes

>Actor: ADMIN, `¿TUTOR?`

>Descripció: Permet eliminar/esborrar alumnes de l'aplicatiu.

## ESTRUCTURA LECTIVA / PLA D'ESTUDIS (ANY ACADÈMIC)

Codi: **STUDIESBROWSE**

>Títol: Cercar/Filtrar/Llistar Estudis

>Actor: ADMIN, TUTOR, DOCENT

>Descripció: Permet cercar, filtrar i llistar els diferents elements de l'estructura d'estudis per codi o nom.

Codi: **STUDIESREAD**

>Títol: Mostrar detalls Estudis

>Actor: ADMIN, TUTOR, DOCENT

>Descripció: Permet veure els detalls i la informació completa d'un element concret de l'estructura lectiva.

Codi: **STUDIESEDIT**

>Títol: Editar Estudis

>Actor: ADMIN

>Descripció: Permet editar/modificar els detalls i la informació dels diferents elements de l'estructura lectiva.

Codi: **STUDIESADD**

>Títol: Afegir Estudis

>Actor: ADMIN

>Descripció: Permet crear/afegir un element a l'estructura lectiva.

Codi: **STUDIESDEL**

>Títol: Eliminar Estudis

>Actor: ADMIN

>Descripció: Permet eliminar/esborrar un element de l'estructura lectiva.

Codi: **STUDIESASSIGN**

>Títol: Assignar Alumne a Estudis [grup(s)/subgrup(s)]

>Actor: ADMIN, TUTOR

>Descripció: Permet assignar/associar els diversos alumnes als grups o subgrups desitjats.

Codi: **STUDIESTEACH**

>Títol: Assignar Docent a Estudis [grup(s)/subgrup(s)]

>Actor: ADMIN

>Descripció: Permet assignar/associar els diversos docents als grups o subgrups desitjats.

## TUTORIES

Codi: **TUTORIABROWSE**

>Títol: Cercar/Filtrar/Llistar Tutories

>Actor: ADMIN

>Descripció: Permet cercar, filtrar i llistar les diferents tutories pel nom assignat (ex.DAW1).

Codi: **TUTORIAREAD**

>Títol: Mostrar detalls Tutories

>Actor: ADMIN

>Descripció: Permet veure els detalls i la informació completa d'una tutoria.

>>Exemple: nom: DAW1, sessió: dilluns 2hores, tutor: Pepito, alumnes: alumne1, alumne2, alumne3, etc...

Codi: **TUTORIAEDIT**

>Títol: Editar Tutories

>Actor: ADMIN

>Descripció: Permet editar/modificar els detalls i la informació de les diferents tutories.

Codi: **TUTORIADD**

>Títol: Afegir Tutories

>Actor: ADMIN

>Descripció: Permet crear/afegir una nova tutoria.

Codi: **TUTORIADEL**

>Títol: Eliminar Tutories

>Actor: ADMIN

>Descripció: Permet eliminar/esborrar una tutoria.

Codi: **TUTORIASSIGN**

>Títol: Assignar Tutor(s) a Tutoria

>Actor: ADMIN

>Descripció: Permet assignar/associar els diversos tutors a les corresponents tutories.

## FALTES

Codi: **FALTABROWSE**

>Títol: Cercar/Filtrar/Llistar Faltes

>Actor: ADMIN, TUTOR, DOCENT

>Descripció: Permet cercar, filtrar i llistar les diferents faltes per el grup/subgrup i sessió.

Codi: **FALTAREAD**

>Títol: Mostrar detalls Faltes

>Actor: ADMIN, TUTOR, DOCENT

>Descripció: Permet veure els detalls i la informació completa d'una falta (ex.sessio, dia, comentaris, alumne, docent).

Codi: **FALTAEDIT**

>Títol: Editar Faltes

>Actor: ADMIN, TUTOR, DOCENT

>Descripció: Permet editar/modificar faltes d'assistència a un alumne concret o un grup/subgrup d'alumnes, canvis contemplats a l'historial.

Codi: **FALTADD**

>Títol: Afegir Faltes

>Actor: ADMIN, TUTOR, DOCENT

>Descripció: Permet crear/afegir faltes d'assistència a un alumne concret o un grup/subgrup d'alumnes (passar llista).

Codi: **FALTADEL**

>Títol: Eliminar Faltes

>Actor: ADMIN, TUTOR

>Descripció: Permet eliminar/esborrar faltes d'assistència a un alumne concret o un grup/subgrup d'alumnes, canvis contemplats a l'historial.

Codi: **FALTAHISTORY**

>Títol: Mostrar Historial Canvis Faltes

>Actor: ADMIN, TUTOR, DOCENT

>Descripció: Permet llistar els canvis realitzats en l'històric de faltes d'assistència.

## IMPORTAR, EXPORTAR CSV (CÀRREGA MASSIVA)

Codi: **IMPORTSTUDIES**

>Títol: Importar Estudis

>Actor: ADMIN

>Descripció: Importar estructura lectiva desitjada junt amb els seus elements mitjançant un document en format .csv (full de càlcul).

Codi: **EXPORTSTUDIES**

>Títol: Exportar Estudis

>Actor: ADMIN

>Descripció: Exportar estructura lectiva desitjada junt amb els seus elements mitjançant un document en format .csv (full de càlcul).

Codi: **IMPORTALUMNE**

>Títol: Importar Alumnes

>Actor: ADMIN, TUTOR

>Descripció: Importar llistat d'alumnes amb l'informacio pertinent: dades personals i de contacte, detalls d'assignació i matricula.

Codi: **EXPORTALUMNE**

>Títol: Exportar Alumnes

>Actor: ADMIN, TUTOR, DOCENT

>Descripció: Exportar llistat d'alumnes amb l'informacio pertinent: dades personals i de contacte, detalls d'assignació i matricula.

Codi: **IMPORTUSER**

>Títol: Importar Usuaris

>Actor: ADMIN

>Descripció: Importar llistat d'usuaris amb l'informacio pertinent: dades personals, d'àcces i de contacte (correu corporatiu) junt amb els detalls d'assignació i d'impartició si escau.

Codi: **EXPORTUSER**

>Títol: Exportar Usuaris

>Actor: ADMIN

>Descripció: Exportar llistat d'usuaris amb l'informacio pertinent: dades personals, d'àcces i de contacte (correu corporatiu) junt amb els detalls d'assignació i d'impartició si escau.

Codi: **IMPORTCONF**

>Títol: Importar Configuració

>Actor: ADMIN

>Descripció: Importar paràmetres de configuració de l'aplicació.

Codi: **EXPORTCONF**

>Títol: Exportar Configuració

>Actor: ADMIN

>Descripció: Exportar paràmetres de configuració de l'aplicació.

Codi: **IMPORTFALTA**

>Títol: Importar Faltes

>Actor: ADMIN, TUTOR, DOCENT

>Descripció: Importar llistat de faltes d'assistència d'una sessió.

Codi: **EXPORTFALTA**

>Títol: Exportar Faltes

>Actor: ADMIN, TUTOR, DOCENT

>Descripció: Exportar llistat de faltes d'assistència d'una sessió.

Codi: **EXPORTREPORT**

>Títol: Exportar Informes

>Actor: TUTOR

>Descripció: Exportar informes descrits a continuació.

## INFORMES

Codi: **RPTALUMNE**

>Títol: Generar Informe Alumne

>Actor: TUTOR

>Descripció: Generar informe d'un alumne concret.

Codi: **RPTALUMNES**

>Títol: Generar Informe Alumnes Tutor

>Actor: TUTOR

>Descripció: Generar informe d'alumnes assignats a un tutor.

Codi: **RPTALUMNES%**

>Títol: Generar Informe Alumnes Percentatge Faltes

>Actor: TUTOR

>Descripció: Generar informe amb els alumnes amb un nombre de faltes superior a percentatge indicat.

Codi: **RPTCURS**

>Títol: Generar Informe Curs

>Actor: TUTOR

>Descripció: Generar informe per un curs concret, inclou totes les classes.

Codi: **RPTCLASSE**

>Títol: Generar Informe Classe

>Actor: TUTOR

>Descripció: Generar informe per una classe concreta, inclou tots els subgrups.

Codi: **RPTSUBGRUP**

>Títol: Generar Informe Subgrup

>Actor: TUTOR

>Descripció: Generar informe per una subgrup concret.

---

**INFORMACIÓ INFORMES**

+ Nombre de Faltes / Retards
	+ Total
	+ Justificades
	+ No Justificades
		+ Hores
+ Comentaris
+ Docents
+ Correccions

## FUNCIONALITATS D'ACCÉS

Codi: **LOGIN**

>Títol: Iniciar Sessió/Accedir a l'Aplicació

>Actor: ADMIN, TUTOR, DOCENT

>Descripció: Accés a l'aplicació mitjançant un usuari (corporatiu) i una contrasenya.

Codi: **REMEMBERPASS**

>Títol: Recordatori Contrasenya

>Actor: ADMIN, TUTOR, DOCENT

>Descripció: Petició recordatori per email corporatiu de la contrasenya (temporal) de l'usuari.

Codi: **CHANGEPASS**

>Títol: Canvi Contrasenya

>Actor: ADMIN, TUTOR, DOCENT

>Descripció: Permet a l'usuari canviar la contrasenya per una de nova.