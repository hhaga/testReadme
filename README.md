Railskurs
=========

Her ligger eksempelapplikasjonen som ble gjennomgått på demoen. Denne kan dere se etter dersom dere ønsker.

Nyttige lenker
--------------
Rails api: <a href="http://api.rubyonrails.org/">http://api.rubyonrails.org/</a>

Oppgaver
--------

Oppgaven går ut på å lage en quiz-applikasjon. Denne må ha oppgaver og alternativer.

1. Velkommen
	- Opprett ein railsapplikasjon som du kaller <b><i>quiz</i></b>
	- Install gemene du trenger
	- Start serveren
	- Sjekk at du får opp ”Welcome aboard”-siden på http://localhost:3000
	 
2. Generer din første scaffold 
	- Bruk rails kommandoen for å generere en scaffold som du kaller <b><i>puzzle</i></b> med disse feltene:
		- <b><i>name</i></b> av typen string
		- <b><i>description</i></b> av typen text
	- Migrer databasen med rake-kommandoen
	
3. Koble sammen entiteter
	- Bruk rails-kommandoen til å generere en ny scaffold som heter <b><i>alternative</i></b> med feltene: 
		- <b><i>answer</i></b> av typen string
		- <b><i>correct</i></b> av typen boolean
		- <b><i>puzzle_id</i></b> av typen integer
	- Migrer databasen med rake-tasken
	- Koble sammen entitetene ved bruk av <b><i>has_many</i></b> og <b><i>belongs_to</i></b>
	- Gjør nødvendige endringer i alternative_controller og views tilhørende puzzle for å få satt alternativene på en bestemt puzzle
	
4. Selve quizen
	- Lag en action i <b><i>puzzle_controller</i></b> med et tilhørende view. Kall det gjerne <b><i>quiz</i></b> 
		- Denne actionen skal hente ut puzzle fra en gitt id som hentes fra objektet som ble sendt inn til actionen
		- Viewet skal rendre puzzleen og tilhørende alternatives
	- Lag enda en action i puzzle_controller som sjekker svarene 
		- Denne actionen må også hente ut puzzle fra en gitt id som hentes fra objektet som ble sendt inn til actionen
		- Pass på at man routes til et gyldig sted når svaret sendes inn

5. Videre arbeid
	- Vi har her satt opp et forslag til utvidelser, men vi har ikke forberedt alternative løsninger til punktene under
		- Autentisering
		- Gå videre til neste spørsmål i quizen
		- Poengberegning
		- CSS

Tips til senere
---------------
Guide for bruk av rails. Går litt mer i dybden på ting enn dette kurset:
<a href="http://guides.rubyonrails.org/">http://guides.rubyonrails.org/</a>

Her kan dere se live-koding av forskjellige Rails-tema:
<a href="http://railscasts.com/">http://railscasts.com/</a>

