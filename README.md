# Oefening disconnected databases : Telefoonboek
## Opdracht
Maak een programma dat telefoonboekgegevens gaat bijhouden in een disconnected database.
## Toelichting
Het programma maakt gebruik van 1 datatable : telefoonnummers.
Deze datatable bevat 4 kolommen : 
-	Nummer, string, max 50, geen null waarden, uniek, primaire sleutel
-	Mobile, byte, standaardwaarde = 1 (0 = geen mobiel toestel, 1 = wel mobiel toestel)
-	Naam, string, max 100, geen null waarden
-	Voornaam, string, max 100

Hoewel je dit waarschijnlijk naar het einde toe gaat programmeren, maar de inhoud (en de structuur) van deze tabel dient bij het afsluiten in een XML bestand bewaard te worden, en bij het opstarten uitgelezen te worden.  
Bestaat dit bestand nog niet, dan dien je de tabelstructuur uiteraard eerst aan te maken.
Bij het opstarten dienen : 
-	grpZoek ingeschakeld te worden
-	lstNummers ingeschakeld te worden
-	grpBewerken zichtbaar gemaakt te worden
-	grpDetails uitgeschakeld te worden
-	btnBewaren en btnAnnuleren onzichtbaar gemaakt te worden

Wanneer we straks op btnNieuw of btnWijzigen gaan klikken dan dienen : 
-	grpZoek uitgeschakeld te worden
-	lstNummers uitgeschakeld te worden
-	grpBewerken onzichtbaar gemaakt te worden
-	grpDetails ingeschakeld te worden
-	btnBewaren en btnAnnuleren zichtbaar gemaakt te worden

lstNummers dient gevuld te worden met Naam + “ “ + voornaam + “ : “ + telefoonnummer.

Telkens een telefoonnummer toegevoegd, gewijzigd of verwijderd wordt dient deze listbox bijgewerkt te worden.

Wordt in lstNummers een item geselecteerd, dan dienen de detailgegevens in de corresponderende controls binnen grpDetails getoond te worden.

Wordt bovenaan in txtZoek een waarde ingevoerd en vervolgens op btnZoek geklikt, dan dient de listbox beperkt te worden tot de items in wiens naam de ingevoerde tekst voor komt.  Wordt op btnEindeZoek geklikt, dan dient txtZoek leeg gemaakt te worden en dienen terug alle items getoond te worden.
