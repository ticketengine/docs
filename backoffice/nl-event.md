# Events
Om een evenement in Ticket Engine aan te maken moeten de volgende 3 stappen worden genomen:
1. Evenement een naam geven en instellen wanneer het evenement plaats vind.
2. Toevoegen van capaciteit.
3. Toevoegen van toegang.

In meer traditionele kaartverkoop systemen moet er voor een evenement "kaartjes" worden aangemaakt. Bij Ticket Engine hebben we gekozen voor toegang, omdat het meer is dan alleen een kaartje. Sommige bezoekers hebben wellicht helemaal geen kaartje nodig. Misschien staan ze op de gastenlijst of hebben ze een lidmaatschap die hun toegang verschaft. Daarom hebben wij gekozen voor het definieren van toegang.


## Details
In dit tabblad kan je de basis gegevens van een evenement beheren.

![alt text][event_details]

Veld | Omschrijving
:--- | :---
Name | Naam van het evenement.
Description | *Optioneel.* Omschrijving van het evenement.
Time frame | De start en eind datum van het evenement.
Tags | *Optioneel.* De tags van het evenement. 

> NOTE: evenementen kunnen alleen wordt geannuleerd en verplaatst als er nog geen kaartjes voor zijn verkocht.


## Capacity
In het capaciteitstabblad kan de voorraad worden beheerd hoeveel plekken er beschikbaar zijn voor het evenement. De capaciteit bestaat uit een Venue (locatie) met 1 of meer capaciteitsgroepen. De capaciteitsgroepen kunnen worden gebruikt om plekken beschikbaar te stellen aan specifieke groepen klanten. 

![alt text][capacity_details]

Veld | Omschrijving
:--- | :---
Location | Naam van de capaciteitsgroep.
Capacity | Aantal beschikbare plekken in de capaciteitsgroep.


## Access
Het toegangstabblad wordt gebruikt voor het definieren van de toegangstypen. In het toegangstype wordt vastgelegd tot welke capaciteitgroep(en) de bezoeker toegang heeft en onder welke voorwaarden de bezoeker toegang kan verwerven.  

![alt text][accesss_details]

Veld | Omschrijving
:--- | :---
Name | Naam van het toegangstype.
Description | *Optioneel.* Omschrijving van het toegangstype.
Access to locations | Capaciteitsgroep(en) waar de bezoeker toegang toe kan krijgen. Als er meer dan 1 groep wordt geselecteerd dan krijgt de bezoeker toegang tot de eerste groep waar nog capacitiets voor beschikbaar is. Voorbeeld: als er 2 groepen (groep A en B) zijn geselecteed, dan krijgt een bezoeker toegang tot groep A totdat deze vol is. Op het moment dat groep A vol is wordt automatisch toegang tot groep B gegeven.
Use limit | Het aantal keren dat de toegang gebruikt kan worden aan de deur. Standaard is de waarde 1, dit betekend dat een kaartje 1 keer geldig is aan de deur. Als dit kaartje nog een keer wordt gescanned zal deze geen toegang krijgen. 
Tags | *Optioneel.* De tags van het toegangstype. 
Conditions | De voorwaarden waar een klant aan moet voldoen om toegang te verwerven voor het evenement. Als een klant moet betalen om naar binnen te mogen is dat ook een voorwaarde waar de klant aan moet voldoen. Dit noemen we een prijs conditie.

### Conditions
De condities zijn de voorwaarden waaraan een bezoeker moet voldoen om toegang te kunnen verwerven voor een evenement. De condities bestaan uit een boom structuur de mogelijkheid om logica toe te voegen d.m.v. "And" en "Or" condities. 

Conditie | Omschrijving
:--- | :---
If | Voeg een nieuwe "And" of "Or" condtie toe.
Price | Definieerd de prijs die een bezoekers moet betalen om toegang te krijgen.
Free entry | Gratis toegang voor een bezoeker. 
Number of items in cart | Het aantal items in de winkelwagen
Cart total value | De totale waarde van de winkelwagen
Sales channel | Het verkoop kanaal waar via de order is geplaatst.
Customer with tag |  
Birth date | De geboordedatum van de bezoeker.
Current date | 

Alle condities hebben de zelfde structuur. Er moet een waarde worden ingevuld en een "operator" zoals "groter dan" of "gelijk aan". De enige uitzondering zijn de prijs condities. Bij een prijs conditie moeten de volgende velden worden ingevuld:

Veld | Omschrijving
:--- | :---
Name | Naam van de prijs.
Currency | De munt eenheid.
Amount | Het bedrag dat moet worden betaald.
Tag | *Optioneel.* De tags van de prijs.
Tax | Belasting over de prijs.
Limit | *Optioneel.* Het maximaal aantal keren dat de prijs conditie gebruikt kan worden.

## Attendees
Het bezoekerstabblad laat een lijst zien van mensen die toegang hebben tot het evenement


[event_details]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/event-detail-edit.png "Event details"
[capacity_details]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/event-capacity-edit.png "Capacity"
[accesss_details]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/event-access-edit.png "Access type"
