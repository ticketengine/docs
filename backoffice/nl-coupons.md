# Coupons
Met coupons kunnen klanten zich identificeren tijdens het bestel process om aangepast prijs condities te activeren.  

## Details
In dit tabblad kan je de basis gegevens van een coupon beheren.

![alt text][coupon_detail]

Veld | Omschrijving
:--- | :---
Name | Naam van de coupon.
Description | *Optioneel.* Omschrijving van de coupon.
Use limit | Het aantal maal dat een coupon code gebruikt kan worden. Gebruik is betekend het aantal kaarten dat er mee gekocht kan worden. 

> NOTE: als een coupon een "use limit" heeft van 1 dan kunnen er 1 kaart met de coupon codes worden gekocht. Als de coupon code wordt ingevuld bij een order maar er worden geen kaarten aan de winkelwagen toegevoegd, dan kan de coupon code nog een keer worden ingevuld bij een andere order.


## Codes
In het codes tabblad kunnen de coupon codes worden beheerd.   

![alt text][coupon_code_list]

### Toevoegen nieuwe coupon codes
Nieuwe coupon codes kunnen op 2 manieren worden aangemaakt. De codes kunnen worden gegenereerd door het systeem of er kunnen codes handmatig worden toegevoegd.

#### Genereren

![alt text][coupon_code_generate]

Veld | Omschrijving
:--- | :---
Number of codes | Het aantal coupon codes dat gegenereerd moet worden.
Code prefix | De tekst waarmee de code moet beginnen. Bijvoorbeeld de prefix partner2020# zal codes opleveren zoals: partner2020#TbVwGqAysJXHZWrqWwTP.

#### Handmatig toevoegen

![alt text][coupon_code_add]

Bij handmatige invoer kunnen codes in het tekstveld worden ingevuld. Als er meerdere codes tegelijk ingevuld worden moeten de codes worden gescheiden door een ; teken. 

### Verwijderen coupon codes
Codes kunnen worden verwijderd d.m.v. het aanvinken van de codes in de lijst. Als er codes zijn aangevinkt verschijnt er een verwijder knop om de codes te verwijderen.

## Coupon condities
Na het aanmaken van een coupon en bijbehorende coupon codes kunnen de coupons worden gebruikt bij het maken van de access condities. Door middel van de conditie "Coupon of type" kan worden afgedwonen welke coupon een klant moet hebben om toegang te krijgen.

![alt text][coupon_condition]


[coupon_detail]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/coupon-detail.png "Coupon details"
[coupon_code_list]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/coupon-code-list.png "Couon list"
[coupon_code_generate]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/coupon-code-generate.png "Coupon code generator"
[coupon_code_add]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/coupon-code-add.png "Coupon code editor"
[coupon_condition]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/coupon-condition.png "Coupon condition"
