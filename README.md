# Rapportage webtoegankelijkheid-test voor openbare bibliotheek van Amsterdam
[live pagina 🌐](https://www.oba.nl/agenda.html)<br/>
[de andere pagina die gecheckt is van de oba](https://github.com/beaupd/oba-activiteitenhub-a11y-audit-autonomous/tree/activiteiten)
![preview oba op digital screen](/assets/unknown.png)

*Dit document is een webtoegankelijkheid-test volgens de Web Content Accessibility Guidelines (WCAG). Een consistente rapportage helpt bij het uitvoeren van een evaluatie en zorgt er voor dat verschilelnde tests kunnen worden vergeleken.*

Datum webtoegankelijkheid-test: 03/11/2021

Webtoegankelijkheid-test uitgevoerd door: Beau & Matthijs

## Inhoudsopgave

  * [Samenvatting](#samenvatting)
  * [Achtergrond bij de evaluatie](#achtergrond-bij-de-evaluatie)
  * [Afbakening](#afbakening)
  * [Beoordelaars](#beoordelaars)
  * [Beoordelingsproces](#beoordelingsproces)
  * [Testresultaten en aanbevelingen](#testresultaten-en-aanbevelingen)
  * [Referenties](#referenties)
  * [Bijlagen](#bijlagen)
  * [Licentie](#licentie)

## Samenvatting

Dit rapport beschrijft in hoeverre de website OBA agendapagina overeenstemt met de *Web Content Accessibility Guidelines (WCAG)* van het W3C. Na de achtergrondinformatie en afbakening van de test worden beoordelaars, beoordelingsproces en testresulltaten beschreven. 

Conclusie van deze test luidt dat de Openbare Bibliotheek Amsterdam website dichtbij voldoet aan de WCAG 2.1, op niveau AA. Gedetailleerde resultaten en aanbevelingen zijn verderop in dit document beschikbaar en in de referenties vindt u bronnen voor eventuele vervolgstudie. Wij stellen feedback op deze evaluatie zeer op prijs.

## Achtergrond bij de evaluatie

De webtoegankelijkheid-test vereist een combinatie van semi-geautomatiseerde en handmatig uitgevoerde evaluatie tools door een ervaren beoordelaar. De beoordelingsresultaten in dit rapport zijn gebaseerd op een beoordeling welke is uitgevoerd op 3-11-2021. De website kan ondertussen aangepast zijn.

## Afbakening

OBA agendapagina

Informatie om deel te nemen aan de informatie samenleving zo laagdrempelig te maken als mogelijk is.

https://www.oba.nl/agenda.html

de agenda pagina is zowel handmatig beoordeeld als met semi-geautomatiseerde tools

03/11/2021

HTML, CSS en javascript

## Beoordelaars

Beau & Matthijs

FDND

Github: beaupd & M4TThys123

Html, Css & javascript

Comfortabel tot proffesioneel.

## Beoordelingsproces

AA

A11y checklist, lighthouse

toegankelijkheidstest aan de hand van A11Y Project-checklist en lighthouse check

## Testresultaten en aanbevelingen

Deze website is dichtbij aan voldoen aan de WCAG 2.1, op niveau AA

### Sterke punten
Sterke punten zijn de leesbaarheid van de content van OBA, en de consistente stijl van de site

### Ontoegankelijke punten
- [user-scalable="no"] is used in the <meta name="viewport"> element or the [maximum-scale] attribute is less than 5.


### Checklist 

Deze website voldoet bijna aan de gehele checklist op een paar punten na. Algehele a11y checklist impressie is boven gemiddeld tot goed

##### Content
  * Het taalgebruik is duidelijk en is eenvoudig te lezen.
  * De inhoud van  de button, a en label elementen zijn uniek en bevatten beschrijvende text. 
  * Op de website is alleen geschikt voor left-to-right talen. Op de website kun je kiezen tussen Nederlands en Engels.


##### Global code
![preview oba op digital screen](/assets/html-checker.png)
  * Een document mag niet zowel een meta-element met een http-equiv-attribuut waarvan de waarde content-type is, als een meta-element met een charset-attribuut bevatten.
``` 
<meta charset="utf-8">
```
 
  * Een meta-element met een http-equiv-attribuut waarvan de waarde X-UA-Compatible is, moet een content-attribuut hebben met de waarde IE=edge.
``` 
<meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
```
 
  * Attribuuttype is op dit moment niet toegestaan bij element selectie.
 ```
 <select id="pagination-selector" type="select" name="pageNumber">
 ```
 
##### Keyboard
  * De interface en inhoud kan worden genavigeerd doormiddel van het toetsenbord.
  * Er is een zichtbare focusstijl voor de geselecteerde elementen via toetsenbordinvoer.
  * De focusvolgorde van het toetsenbord komt overeen met de visuele lay-out.

##### Images
  * Zorg ervoor dat alle img-elementen een alt-attribuut hebben.
  * Bij bijna alle img-elementen van agenda pagina ontbreken de alt-attributen. Alleen het logo van OBA bevat een alt-attribuut.
   ```
<img src="/content/dam/logo/oba-logo.png" alt="Openbare Bibliotheek Amsterdam">
```

##### Headings
* Er is geen h1.
* De h2 elementen hebben niet de zelfde ```font-size```. (had handig geweest als de grootste text een h1 zou zijn)
* De headings beschrijven goed de content van de pagina.
* Er is verder een logische opbouw omdat de geneste headings een waarde hebben van h3.

##### Lists
* De nav, filter-nav, agenda & footer-nav bevatten allemaal een unordered list.
* De pagina-nav bestaat uit een ordered list.
* Alle lists zijn correct genest.

##### Controls
* Alle links & knoppen zijn toegankelijk voor screenreaders en keyboard navigatie.

##### Tables
n.v.t.

##### Forms
- All inputs in a form are associated with a corresponding label element.<br />
 	Elke input of selection heeft label met for property
- Use fieldset and legend elements where appropriate.<br />
 	n.v.t.
- Inputs use autocomplete where appropriate.<br />
 	n.v.t.
- Make sure that form input errors are displayed in list above the form after submission.<br />
 	n.v.t.
- Associate input error messaging with the input it corresponds to.<br />
 	n.v.t.
- Make sure that error, warning, and success states are not visually communicated by just color.<br />
 	n.v.t.

##### Media
- Make sure that media does not autoplay.<br />
 	n.v.t.
- Ensure that media controls use appropriate markup.<br />
 	n.v.t.
- Check to see that all media can be paused.<br />
 	n.v.t.

##### Video
- Confirm the presence of captions.<br />
 	n.v.t.
- Remove seizure triggers.<br />
 	n.v.t.

##### Audio
- Confirm that transcripts are available.<br />
 	n.v.t.

##### Appearance
- Check your content in specialized browsing modes.<br />
	 In zowel high contrast mode als inverted color mode ziet de site er nog steeds goed uit en is de content te lezen.
- Increase text size to 200%.<br />
 	Niks overlapt en alles is nog leesbaar
- Double-check that good proximity between content is maintained.<br />
 	Alle content is nog steeds makkelijk te ontdekken
- Make sure color isn't the only way information is conveyed.<br />
 	Ja alles is nog steeds te vinden in grayscale
- Make sure instructions are not visual or audio-only.<br />
 	De namen van de secties en elementen zijn descriptieve en duidelijk genoeg
- Use a simple, straightforward, and consistent layout.<br />
 	Redelijk simpele generieke layout, consistent wel erg complex en groot.

##### Animation
- Ensure animations are subtle and do not flash too much.<br />
	 n.v.t.
- Provide a mechanism to pause background video.<br />
 	n.v.t.
- Make sure all animation obeys the prefers-reduced-motion media query.<br />
 	n.v.t.

##### Color contrast
- Check the contrast for all normal-sized text.<br />
  Het is zwart op wit en er is genoeg contrast
- Check the contrast for all large-sized text.<br />
 	Het is zwart op wit en er is genoeg contrast
- Check the contrast for all icons.<br />
 	Het is rood op wit en er is genoeg contrast
- Check the contrast of borders for input elements (text input, radio buttons, checkboxes, etc.).<br />
 	Het is allemaal een tint van grijs en er is gezorgd voor genoeg contrast
- Check text that overlaps images or video.<br />
 	Er is geen text dat images of videos overlapt
- Check custom ::selection colors.<br />
 	Is een tint van grijs en is genoeg contrast


##### Mobile and touch
- Check that the site can be rotated to any rotation.<br />
  The site allows both orientations on mobile
- Remove horizontal scrolling.<br />
  The site has no horizontal scrolling
- Ensure that button and link icons can be activated with ease.<br />
  De buttons van de sites en links zijn groot genoeg en toegankelijk
- Ensure sufficient space between interactive items in order to provide a scroll area.<br />
 	n.v.t.
[user-scalable="no"] is used in the <meta name="viewport"> element or the [maximum-scale] attribute is less than 5.
Users kunnen niet echt zoomen op de mobiel. Uit de lighthouse check gebleken

### Light House check mobile
![lighthouse Check](/assets/lighthouseCheck.png)

### Light House check desktop
![lighthouse Check](/assets/lighthouseCheckDesktop.png)

{Neem links op naar de WCAG 2.1 succescriteria en technieken voor de ontoegankelijke punten}

{Voeg per check specifieke rapportage(s), of links naar rapportage(s) toe in de Wiki, bv. screenshots van tests}

[user-scalable="no"] naar [user-scalable="yes"] veranderen zodat de user kan inzoomen. Bepaald met de lighthouse Check
{Schrijf per check aanbevelingen voor het verbeteren van ontoegankelijke punten}

{Beschrijf of verwijs per check naar een programma voor het monitoren van webstite toegankelijkheid, her-beoordeling aan de hand van beoordelingsinstrumenten etc.}

### Resultaten Usability test

{Beschrijf per pagina de bevindingen uit jouw usability test in het lab.}

## Referenties

Referenties welke gebruikt zijn bij de webtoegankelijkheid-test. Deze referenties zijn allen in het Engels:

- [Overzicht en introductie van de Web Content Accessibility Guidelines (WCAG)](https://www.w3.org/WAI/intro/wcag)
- [De complete Web Content Accessibility Guidelines 2.1 (WCAG)](https://www.w3.org/TR/WCAG21/)
- [Technieken voor WCAG 2.1](https://www.w3.org/WAI/WCAG21/Techniques/)
- [Bronnen voor beoordeling van webtoegankelijkheidsevaluatie ](http://www.w3.org/WAI/eval/)
- [Tools lijst voor semi-geautomatiseerde beoordeling van webtoegankelijkheid](https://www.w3.org/WAI/ER/tools/)
- [Informatie over het gebruik van gecombineerde expertise voor het evalueren van webtoegankelijkheid](https://www.w3.org/WAI/eval/reviewteams)
- [A11Y Project Checklist](https://www.a11yproject.com/checklist/)

## Bijlagen
