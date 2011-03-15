Railskurs
=========

Her ligger eksempelapplikasjonen som ble gjennomgått på demoen. Denne kan dere se etter dersom dere ønsker.


Oppgaver
--------

Oppgaven går ut på å lage en quiz-applikasjon. Denne må ha oppgaver og alternativer.

1. Oppgave 1: Velkommen
	- Opprett ein railsapplikasjon som du kaller quiz
	- Install gemene du trenger
	- Start serveren
	- Sjekk at du får opp ”Welcome aboard”-siden på http://localhost:3000
	 
2. Oppgave 2 – Generer din første scaffold 
	- Bruk rails kommandoen for å generere en scaffold som du kaller <b><i>puzzle</i></b> med disse feltene:
		- <b><i>name</i></b> av typen string
		- <b><i>description</i></b> av typen text
	- Migrer databasen med rake-kommandoen
	
3. Oppgave 3 - Koble sammen entiteter
	- Bruk rails-kommandoen til å generere en ny scaffold som heter <b><i>alternative</i></b> med feltene: 
		- <b><i>answer</i></b> av typen string
		- <b><i>correct</i></b> av typen boolean
		- <b><i>puzzle_id</i></b> av typen integer
	- Migrer databasen med rake-tasken
	- Koble sammen entitetene ved bruk av <b><i>has_many</i></b> og <b><i>belongs_to</i></b>
	- Gjør nødvendige endringer i alternative_controller og views tilhørende puzzle for å få satt alternativene på en bestemt puzzle
 
