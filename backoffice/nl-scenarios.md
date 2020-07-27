# Voorbeeld verkoop scenario's



## Selecte groep klanten mag eerder kopen d.m.v. een coupon code
Het is mogelijk om een bepaalde groep klanten (bijvoorbeeld vrienden van het festival of theater) eerder de mogelijkheid te geven om kaarten te kopen voor een voorstelling. Je kan deze mogelijkheid bieden door deze groep klanten een coupon code te geven. De overige klanten kunnen vanaf een bepaalde datum pas een kaartje kopen.

Bij dit scenario ga we er van uit dat er al een voorstelling en een coupon zijn aangemaakt.

[Hoe maak ik een voorstelling aan?](https://github.com/ticketengine/docs/blob/master/backoffice/nl-event.md)
 
[Hoe maak ik een coupon aan?](https://github.com/ticketengine/docs/blob/master/backoffice/nl-coupons.md)  

### Scenario overzicht
- Vrieden kunnen eerder een kaartje kopen d.m.v. een coupon code.
- Regulier publiek kan een kaartje kopen vanaf een bepaalde datum.

### Hoe richt je het scenario in?
- Ga naar de event pagina en klik op de access tab.
- Voeg een nieuw access type toe.
![alt text][add-access]
- Vul de access gegevens in en vul bij condities de reguliere prijs in.
![alt text][new-access] 

We hebben nu een toegang met een reguliere prijs. Maar we moeten er voor zorgen dat deze reguliere verkoop pas vanaf een bepaalde datum beschikbaar is.

- Klik op het plus icoontje naast de "Reguliere" prijs om een extra conditie voor deze prijs toe te voegen.
![alt text][scenario-vrienden-coupon-2]
- Kies voor een "Current date" conditie.
![alt text][new-condition-current-date]
- Selecteer "Is greater-then or equal to" en kies een datum vanaf wanneer de reguliere verkoop start. Als het goed is ziet het er dan zo uit: 

![alt text][condition-price-from]

We hebben nu een reguliere prijs die gekocht kan worden vanaf een vastgestelde datum. Nu moeten we een tarief aanmaken die met een coupon kan worden aangeschaft

- Klik het plus icoontje onderaan om een nieuwe prijs toe te voegen.
![alt text][scenario-vrienden-coupon-3]
- Kies voor "Price" en vul de prijs in en een naam voor het tarief, bijvoorbeeld "Vrienden".
![alt text][condition-add-new-price]
- Klik het plus icoontje naast de "Vrienden" prijs om een nieuwe conditie aan de prijs toe te voegen.
![alt text][scenario-vrienden-coupon-4]
- Kies voor "Coupon of type".
- Selecteer "Contains" en kies vervolgens de aangemaakte coupon die ingevuld moet worden. Als het goed is zien de condities er dan als volgt uit:

![alt text][scenario-vrienden-coupon-5]
- Klik op "Save" onderaan de pagina om de access op slaan.  



## Early bird, een gereduceerde prijs als er voor een bepaalde datum wordt gekocht
Bij dit scenario ga we er van uit dat er al een voorstelling en een coupon zijn aangemaakt.

[Hoe maak ik een voorstelling aan?](https://github.com/ticketengine/docs/blob/master/backoffice/nl-event.md)
 
[Hoe maak ik een coupon aan?](https://github.com/ticketengine/docs/blob/master/backoffice/nl-coupons.md)  

### Scenario overzicht
- Voor een vastgestelde datum geld er een gereduceerd tarief.
- Na deze datum geld er een regulier tarief.

### Hoe richt je het scenario in?
- Ga naar de event pagina en klik op de access tab.
- Voeg een nieuw access type toe.
![alt text][add-access]
- Vul de access gegevens in en vul bij condities de reguliere prijs in.
![alt text][new-access] 

We hebben nu een toegang met een reguliere prijs. Maar we moeten er voor zorgen dat deze reguliere verkoop pas vanaf een bepaalde datum beschikbaar is.

- Klik op het plus icoontje naast de "Reguliere" prijs om een extra conditie voor deze prijs toe te voegen.
![alt text][scenario-vrienden-coupon-2]
- Kies voor een "Current date" conditie.
![alt text][new-condition-current-date]
- Selecteer "Is greater-then or equal to" en kies een datum vanaf wanneer de reguliere verkoop start. Als het goed is ziet het er dan zo uit: 

![alt text][condition-price-from]

We hebben nu een reguliere prijs die gekocht kan worden vanaf een vastgestelde datum. Nu moeten we het "Early bird" tarief aanmaken.

- Klik het plus icoontje onderaan om een nieuwe prijs toe te voegen.
![alt text][scenario-vrienden-coupon-3]
- Kies voor "Price" en vul de prijs in en een naam voor het tarief, bijvoorbeeld "Early bird".
![alt text][condition-add-new-price]
- Klik het plus icoontje naast de "Early bird" prijs om een nieuwe conditie aan de prijs toe te voegen.
![alt text][scenario-early-bird-2]
- Kies voor een "Current date" conditie.
- Selecteer "Is less-then" en kies een datum tot wanneer de "Early bird" verkoop loopt. Als het goed is ziet het er dan zo uit:
 
![alt text][scenario-early-bird-3]


[add-access]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/add-access.png "Add access"
[new-access]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/new-access.png "New access"
[condition-price-from]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/condition-price-from.png "-"
[condition-add-new-price]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/condition-add-new-price.png "New price condition"
[new-condition-current-date]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/new-condition-current-date.png "New cureent date condition"
[scenario-vrienden-coupon-1]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/scenario-vrienden-coupon1.png "Coupon details"
[scenario-vrienden-coupon-2]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/scenario-vrienden-coupon2.png "Coupon details"
[scenario-vrienden-coupon-3]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/scenario-vrienden-coupon3.png "Coupon details"
[scenario-vrienden-coupon-4]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/scenario-vrienden-coupon4.png "Coupon details"
[scenario-vrienden-coupon-5]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/scenario-vrienden-coupon5.png "Coupon details"
[scenario-early-bird-1]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/scenario-early-bird-1.png "Coupon details"
[scenario-early-bird-2]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/scenario-early-bird-2.png "Coupon details"
[scenario-early-bird-3]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/scenario-early-bird-3.png "Coupon details"