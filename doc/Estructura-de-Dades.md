Estructura de Dades
===================

Tractarem les dades de forma esquematica, representades en format JSON (JavaScript Object Notation) i anomenarem els diferents components de dades (designats documents) com a objectes d'una collecció en una base noSQL o no relacional.

Ens hem decantat per aquest sistema de gestió de bases de dades per poder així obtenir una millor escalabilitat de la mateixa, a més aquest sistema no ens obliga a mantenir estructures fixes com es el cas de les taules en d'altres sistemes gestors relacionals. Això es considera idoni sobretot en la conformació de l'estructura lectiva que volem crear i ens ofereix flexivilitat de cara al futur. Finalmnet ens dona un avantatge a l'hora d'enmagatzemar i registrar events, tractant-se d'una aplicació per la gestio de faltes d'assistència

A continuació mostrarem l'estructura de les diferents colleccions, veurem que l'estructura d'un document es senzilla i esta composta per "key-value", clau-valor, on la clau es el nom del camp i el valor el seu contingut. Aquestes estan separades mitjançant ":" i manté com em dit al principi el format JSON.

## Estudis

	//"id": "4b93d6f1da357cdeec678514",
	{
		"anyacademic": "2012-2013",
		"curs": [
			{
				"codi": "DAW",
				"nom": "Desenvolupament d'Aplicacions Web",
				"tutoria": [
					{
						"nom": "DAW1",
						"tutors": ["id Ambrosio A", "id Fulanito C"],
						"sessions": [
							{"dia": "dilluns", "hores": 2}
						]
					},
					{
						"nom": "DAW2",
						"tutors": ["id Ambrosio B"],
						"sessions": [
							{"dia": "divendres", "hores": 2}
						]
					}
				],
				"classe": [
					{
						"codi": "M01UF1",
						"nom": "Instal·lació, configuració i explotació del sistema informàtic",
						"hores": 60,
						"subgrup": [
							{"nom": "A", "docent": "id Ambrosio A"}
						]
					},
					{
						"codi": "M01UF2",
						"nom": "Gestió de la informació i de recursos en una xarxa",
						"hores": 80,
						"subgrup": [
							{
								"nom": "A",
								"assignacio": [
									{"docent": "id Menganito A"},
									{"docent": "id Menganito Sustitut", "periode_inici": "2013-02-17", "periode_fi": "2013-03-17"}
								],
								"sessions": [
									{"dia": "dilluns","hores": 2},
									{"dia": "dijous", "hores": 2},
									{"dia": "divendres", "hores": 1}
								]
							},
							{"nom": "B", "docent":"Menganito B"}
						]
					},
					{
						"codi": "M01UF3",
						"nom": "Implantació de programari específic",
						"hores": 25,
						"subgrup": [
							{"nom": "A", "docent": "id Fulanito A"},
							{"nom": "B", "docent": "id Fulanito B"},
							{"nom": "C", "docent": "id Fulanito C"}
						]
					},
					{
						"codi": "M02UF1",
						"nom": "Introducció a les bases de dades",
						"hores": 33,
						"subgrup": [
							{"nom": "A", "docent": "id Pacoporras A"}
						]
					},
					{
						"codi": "M02UF2",
						"nom": "Llenguatges SQL: DML i DDL",
						"hores": 66,
						"subgrup": [
							{"nom": "A", "docent": "id Jaimito A"},
							{"nom": "B", "docent": "id Jaimito B"}
						]
					},
					{
						"codi": "M02UF3",
						"nom": "Llenguatges SQL: DCL i extensió procedimental",
						"hores": 66,
						"subgrup": [
							{"nom": "A", "docent": "id Peret A"}
						]
					},
					{
						"codi": "M02UF4",
						"nom": "Bases de dades objectes-relacionals",
						"hores": 33,
						"subgrup": [
							{"nom": "A", "docent": "id Licensiado A"}
						]
					}
				]
			}
		]
	}

## Alumnes

	{
		"dni": "12345678T",
		"nom": "pepe",
		"cognoms": "garcia perez",
		"email": "pepe@email.com",
		"tel": "666 666 666",
		"matriculat": [
			{
				"anyacademic": "2012-2013",
				"curs": [
					{
						"codi": "DAI",
						"tutoria" : "DAI1",
						"classes": [
							{"codi": "M01UF1"},
							{
								"codi": "M01UF2",
								"subgrup": "A",
								"faltes": [
									{"dia": "2012-11-12" , "hores": 1},
									{"dia": "2013-02-28" , "hores": 2, "justificada": true},
									{"dia": "2013-04-05" , "retard": 1}
								]
							}
						]
					},
					{
						"codi": "DAW",
						"tutoria" : "DAW1",
						"classes": [
							{"codi": "M01UF1"}
						]
					},
					{
						"codi": "SMX",
						"tutoria" : "SMX2"
					}
				]
			}
		]
	}

## Docents

	{
		"nom": "Ana",
		"cognoms": "Riu",
		"email": "ana.riu@iesjoandaustria.org",
		"login": {
			"usuari": "ana.riu",
			"password":"password",
			"admin":true
		},
		"rols": [
			{"rol":102},
			{"rol":103}
		]
	}