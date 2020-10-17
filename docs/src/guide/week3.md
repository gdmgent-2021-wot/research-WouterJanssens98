# Week 3

## Opbouw van een AR project

### Modellen

![3D Models](https://free3d.com/imgd/l86/5c942b6e26be8b19238b4567/6725-amphibious-blender-28.jpg)

Een 3D-model ligt steeds aan de basis van een AR-project. Deze 3D-modellen bevatten alle info om zodanig gebruikt te worden dat deze mits verwerking in code perfect aan sluiten bij de ruimte waarin men de AR-technologie toepast. De software om deze 3D modellen te maken is sterk uiteenlopend. Het vinden van een 3D-model van een bepaald object of personage is meestal eenvoudig, maar het maken van een nauwkeurig model is vrij moeilijk, vooral als het model in Augmented Reality gebruikt moet worden. Gezien het grote gebruik van 3D-middelen vandaag, is er een grote vraag naar 3D-modellering, vooral in de beperkte niche van augmented reality.


Een van de belangrijkste zaken voor iemand die AR-ready 3D-modellen nodig heeft, is het platform waarop ze zullen worden gebruikt. Het is redelijk vanzelfsprekend dat een gamepersonage gedetailleerder moet zijn dan een model die op onze smartphone wordt weergegeven. Welke beslissingen moeten er dan gemaakt worden? Hier zal ik even dieper op ingaan.


Hoewel de meeste AR-toepassingen ontwikkeld zijn voor mobiele applicaties, stijgt het aantal applicaties voor draagbare gadgets veel sneller. Meestal zijn deze applicaties gebouwd voor smartglasses: een draagbare bril met een ingebouwd display. De meest bekende voorbeelden van deze brillen zijn de Vuzix Blade, Google Glass en Dreamglass.


#### Platform
Op basis van het platform waarop ze zijn afgestemd, vereisen AR-toepassingen verschillende soorten 3D-modellen. Mobiele apps hebben bijvoorbeeld de neiging om kleinere en minder gedetailleerde ontwerpen te hebben dan die aanwezig in applicaties voor smartglasses. Dit komt omdat smartphones en tablets een veel kleiner gezichtsveld en schaal hebben dan smartglasses, dus is het niet nodig om een ​​detailniveau toe te voegen dat de gebruiker toch niet zal opmerken.

Daarnaast is het ook interessant om te vermelden dat 3D-modellen vaak gebouwd zijn met de interactie als doel. Voor mobiele apps vindt de interactie meestal plaats door simpelweg te tikken en de positie van je smartphone te veranderen, terwijl apps voor smartglasses tekst en objecten kunnen bevatten die reageren op acties in het gezichtsveld van de gebruiker (zoals proberen ze met een hand aan te raken).


## Opbouw van een 3D Model

![Opbouw](https://cloud.addictivetips.com/wp-content/uploads/2009/01/3dmodelmadewithblender.jpg)

Over het algemeen moet je geen expert zijn of voorkennis hebben om een ​​3D-model voor Augmented Reality te maken, maar om het er mooi uit te laten zien en goed te laten functioneren is kennis & ervaring vaak wel een must. Het importeren van een simpel 3D model zal eveneens leiden tot een AR-applicatie die er simpel uitziet.

Er bestaan verschillende manieren om AR-ready 3D-middelen te maken. Vroeger gebeurde dit met de  fotogrammetrie (waarbij het model wordt gemaakt op basis van een reeks foto's), scannen (een object wordt gescand, digitaal gemaakt en de extra dimensie van volume wordt toegevoegd), maar de meest huidige oplossing tegenwoordig is door het gebruik van software. Er bestaan tal van programma's voor 3D-ontwerp, met zowel gratis opties (zoals Blender en SketchUp) als betaalde opties (zoals Maya en Houdini) om uit te kiezen.

Hieronder zal ik even kort samenvatten welke de voor- en nadelen zijn van voorgaande software.

### Blender

#### Voordelen

* Gratis & open source software
* Veel gratis modellen
* Enorm veel tools & en tutorials om snel te groeien in 3D modelling


#### Nadelen

* Redelijk imposante interface met veel knopjes -> moeilijk voor onervaren gebruikers
* Niet altijd ondersteund voor implementatie met andere programma's
* Geen industrie standaard - niet echt professioneel gebruikt

[![Blender](http://img.youtube.com/vi/CSc_aH25cUY/0.jpg)](https://www.youtube.com/watch?v=CSc_aH25cUY "Blender")


### Maya

#### Voordelen

* Zeer goed in animatie
* Wordt professioneel gebruikt
* Vrije-vorm benadering van 3D-modellering - makkelijker dan de meeste 3D-modelling programma's


#### Nadelen

* Betalend - $1470/jaar
* Soms compatibiliteitsproblemen
* Duurt lang om het volledig onder de knie te krijgen



## Uitleg & Live voorbeeld  

Ik was van plan om voor deze les een Snapchat filter te maken aan de hand van Augmented Reality, maar aan   gezien deze moet goedgekeurd worden & ik pas eergisteren begonnen was koos ik om jullie een ander live voorbeeld te tonen. Hierbij een korte tutorial om jullie eigen 3D-modellen uit Blender weer te geven binnen een ruimte.


### Stappenplan

1. 3D Model modelleren in Blender of andere software

2. Exporteren als Wavefront object

3. Bij gebruik van materials extra export voorzien door middel van een .mtl (material) file

4. Bij gebruik van textures extra export voorzien voor "textures" folder

5. Bestanden zippen & uploaden bij AR-applicatie




[Live Voorbeeld](https://www.screenleap.com/drerman98)