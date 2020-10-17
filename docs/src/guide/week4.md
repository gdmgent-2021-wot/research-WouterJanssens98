# Week 4

## Creatie van een AR-ervaring

### Manual

Met deze 'manual' leg ik voor jullie uit hoe je zelf AR-technologie kan toepassen aan de hand van code & je mobiele toestel.

![Foto](https://tr1.cbsistatic.com/hub/i/r/2019/12/16/4ff17863-74c6-425a-be4a-42e245fd272f/resize/1200x/d63ead87cc8b3f586acb3cb42022456c/istock-1126094461.jpg)


1. Beginnen met een propere lei -> aanmaken van een nieuwe folder, zijnde "Voorbeeld AR".

![Folder](/images/2.png)


2. Aanmaken van een index.html bestand

![HTML](/images/1.png)

2. Toevoegen van het AR.JS & A-Frame framework

![Frameworks](/images/3.png)

#### AR.JS

AR.js is een bibliotheek voor Augmented Reality op het web, met functies als Image Tracking, Location-based AR en Marker tracking.

Er bestaan twee versies van AR.JS, elk met hun eigen opbouw & code. Slechts 1 versie kan geïmporteerd worden per project.

1. AR.js met Image Tracking & Location Based AR:


2. AR.js met Marker Tracking & Location Based AR

In dit voorbeeld zal ik gebruik maken van Marker Tracking in plaats van Image Tracking, aangezien deze beter werkt bij belichting & minder scherpe camera's.


#### A-Frame.JS

Afhankelijk van de versie van AR.js wordt er een andere versie van A-Frame gebruikt.

A-Frame is een webframework voor het bouwen van virtual reality (VR)-ervaringen. Het is gebaseerd op HTML, waardoor het eenvoudig is om aan de slag te gaan. A-Frame is niet alleen een 3D-scèneframework of een opmaaktaal; het is een taal die vooral structuur biedt voor three.js.

#### Bouwen van een scene

Binnen de body van ons HTML bestand creëren we een 'scene', waarin we dus AR-tracking kunnen definieren.


![Scene](/images/4.png)


Deze scenen geven we 3 attributen mee : 

1. Stats -> weergeven van stats zoals o.a. fps op het scherm

2. Embedded -> weergeven van het frame binnen deze HTML code

3. AR.js -> creëren van een A-frame scene aan de hand van AR.JS


Het AR.JS attribuut krijgt daarnaast ook parameters.

* trackingMethod : best -> beste/meest intensieve methode voor het herkennen van markers -> meest accuraat
* debugUIEnabled : false -> aangezien wij NMD'ers feilloos kunnen programmeren is debuggen helemaal niet nodig!



#### Toevoegen van de AR-herkenning

AR-herkenning met AR.js kan op verschillende manieren gebeuren, zijnde :

* Hiro -> default marker binnen AR.js

![Hiro](https://upload.wikimedia.org/wikipedia/commons/4/48/Hiro_marker_ARjs.png)

Tegenhanger van Hiro : Kanji

![Kanji](https://www.researchgate.net/profile/Gabor_Sziebig/publication/235768408/figure/fig1/AS:472510123778049@1489666600407/Example-for-a-marker-with-kanji-as-a-pattern.png)


* Barcode -> Automatisch gegenereerde markers dankzij matrixbewerkingen.

Kan je ook zelf genereren zodat je zelf een unieke marker hebt!

![Generator](/images/5.jpg)


* Pattern -> Op basis van een foto zelf een pattern genereren (.patt bestand).

Nadelen : vaak niet accuraat bij ingewikkelde foto's / logo's

![Marker](/images/6.png)

Hierbij wordt de Hiro marker gebruikt als herkenning.

#### Toevoegen van een interface

De A-Frame interface ondersteunt meerdere toepassingen om de AR-technologie toe te passen.

##### AR-gerelateerd

* Kubus
* Foto
* Cirkel
* Cillinder
* Video
* ....


##### Niet AR-gerelateerd

* Geluid 
* Link naar website (zoals QR)
* Openen van applicaties
* ...


In dit voorbeeld zal ik zowel een foto als kubus gebruiken binnen de A-Frame.


#### Toevoegen van het object

##### Kubus

![Kubus](/images/7.png)

De kubus met als tag `<a-box>` krijgt op zijn beurt meerdere attributen.

* Position : de positie gezien ten opzichte van de marker. In dit geval wordt de kubus over een eenheid van "1" uit de marker geduwd, naar jezelf toe dus.

* Material : het definiëren van materiaalkenmerken. In dit geval : de kleur rood toevoegen aan het oppervlak van de kubus.

#### Foto

![Foto](/images/10.png)

De foto met als tag `<a-image>` krijgt net zoals de kubus meerdere attributen.

* SRC : path naar de foto 

* Positon : idem kubus : dichter naar jezelf toe

* Rotation : ieder object wordt standaard ingeladen met de voorkant van het object richting de grond. Een rotatie van 270° om zijn as zorgt er dus voor dat dit voor ons op de juiste positie komt te staan.



#### Lokaal hosten 

Om onze toepassing online te krijgen, maken we gebruik van de npm-module genaamd "http server".

Deze installeren we door middel van volgende code uit te voeren

`npm install -g http-server`

Eens geïnstalleerd starten we de server doormiddel van volgend commando

`http-server`

#### Online hosten

De laptopcamera gebruiken is redelijk omslachtig met AR, vandaar dat we deze eerst online zullen hosten.

Dit doen we aan de hand van NGROK.

![NGrok](/images/8.png)

Ngrok zal de lokale server die op je laptop runt omzetten (via tunneling) naar een beveiligd ngrok adress dat je kan gebruiken als testomgeving.

Na het downloaden & openen van Ngrok activeren we deze server op de volgende manier :

`ngrok http 8080`

Op deze manier zal de lokale server op poort 8080 nu ook gehost worden op een ngrok adres.

![Running](/images/9.png)

Ngrok geeft ons echter twee opties, een http en een https adres. Tijdens de uitvoering van mijn project ben ik erachter gekomen dat enkel https zal werken met AR.js, aangezien de toestemming voor camera enkel gevraagd wordt bij een beveiligde verbinding, zijnde HTTPS.

We kopiëren deze https link & openen deze, bij voorkeur, in een chrome browser op ons mobiel toestel. 


#### Testen van de code


Eens we de link openen in een browser op een mobiel toestel, met voorkeur Chrome, zal er gevraagd worden om cameratoegang.

Zodra deze verleend wordt is onze mobiele applicatie klaar om markers te herkennen!

### LIVE DEMO


[Live Voorbeeld](https://www.screenleap.com/drerman98)


































