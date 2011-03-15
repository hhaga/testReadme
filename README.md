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
	- Bruk rails kommandoen for å generere en scaffold som du kaller <b><u>puzzle</u></b> med disse feltene:
		- <b><u>name</u></b> av typen string
		- <b><u>description</u></b> av typen text
	- Migrer databasen med rake-kommandoen
	
3. Oppgave 3 - Koble sammen entiteter
	- Bruk rails-kommandoen til å generere en ny scaffold som heter <b><u>alternative</u></b> med feltene: 
		- <b><u>answer</u></b> av typen string
		- <b><u>correct</u></b> av typen boolean
		- <b><u>puzzle_id</u></b> av typen integer
	- Migrer databasen med rake-tasken
	- Koble sammen entitetene ved bruk av <b><u>has_many</u></b> og <b><u>belongs_to</u></b>
	- Gjør nødvendige endringer i alternative_controller og views tilhørende puzzle for å få satt alternativene på en bestemt puzzle
 
