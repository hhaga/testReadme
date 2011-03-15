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
	- Bruk rails kommandoen for å generere en scaffold som du kaller <b>puzzle</b> med disse feltene:
		- name av typen string
		- description av typen text
	- Migrer databasen med rake-kommandoen
	
3. Oppgave 3 - Koble sammen entiteter
	- Bruk rails-kommandoen til å generere en ny scaffold som heter alternative med feltene: 
		- answer av typen string
		- correct av typen boolean
		- puzzle_id av typen integer
	- Migrer databasen med rake-tasken
	- Koble sammen entitetene ved bruk av has_many og belongs_to
	- Gjør nødvendige endringer i alternative_controller og views tilhørende puzzle for å få satt alternativene på en bestemt puzzle
 
