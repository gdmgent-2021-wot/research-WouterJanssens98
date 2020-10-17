# Week 2

##  Eigen visie binnen Augmented Reality

![Groei AR](https://s27389.pcdn.co/wp-content/uploads/2018/05/Project-Growth.png)


Zoals op bovenstaande grafiek duidelijk wordt aangetoond is de AR-markt ééntje om wel in de gaten te houden! Steeds meer technologiebedrijven brengen apps op de markt, voorzien simpele applicaties of verwerken AR-gebruik in hun verkoopsmethode (cfr. IKEA). Met de release van iOS11 & zijn eigen "AR-kit" komt Augmented Reality steeds dichter bij de particulier & geraakt deze hiermee vertrouwd. Volgens Google is mobiele AR één van de meest evoluerende trends van het laatste jaar. Het aantal toestellen dat AR ondersteunt stijgt namelijk exponentieel. Het doel dat men in de toekomst voor ogen heeft bestaat eruit Machine Learning / Artificial Intelligence te linken aan Augmented Reality. Op deze manier zal de technologie zich steeds kunnen uitbreiden & biedt dit veel mogelijkheden voor de toekomst.


Het enorme succes van Pokemon Go bewees dat deze evolutie niet weg te denken was. Daarnaast is het waarschijnlijk het eerste dat in ons opkomt als we aan Augmented Reality denken. Sinds de komst van Pokémon Go hebben veel bedrijven zich hierop toegespitst/uitgebreid. Denk maar aan Ikea Home, Google Lens, Snapchat, ... . 



![Verdeling Markt](https://s27389.pcdn.co/wp-content/uploads/2018/05/AR-Industry.png)

De verdeling van de markt geeft een goed inzicht in de sectoren waar AR reeds goed geïmplementeerd is. Hierbij kan men eveneens besluiten dat er in bepaalde sectoren nog zeer veel mogelijkheid is tot uitbreiden. Op het vlak van educatie bijvoorbeeld. Aangezien we nog geen Augmented Reality gebruiken binnen onze opleiding aan de Artevelde Hogeschool, zal ik hiervoor een implementatie voorzien.

## AR.JS

De simpelste manier om Augmented Reality te integreren op het web is zonder twijfel AR.JS. De implementatie wordt voorzien in de webbrowser, wat betekent dat er geen app hoeft geïnstalleerd te worden. Daarnaast werkt het op alle mobiele platforms: Android, iOS11 en Windows Mobile. Een telefoon volstaat dus om hiervan gebruik te maken. 

### Voordelen
* Open Source
* Hoge fps, zelfs op verouderde toestellen
* Cross Platform / Werkt op praktisch iedere telefoon
* Simpliciteit van het project

### VIDEO

[![AR.JS](http://img.youtube.com/vi/hdXY1tFQ2Hw/0.jpg)](http://www.youtube.com/watch?v=hdXY1tFQ2Hw "AR.JS")



##  Link met New Media Development

Voor het vak Extended Reality bouwden we reeds enkele kleine 3D Blender modellen. Deze kunnen via de app & plugin Augment geïntegreerd worden in je woonkamer. Dit is iets dat ik voor dit project ongetwijfeld zal uitwerken & testen / een beknopte handleiding voor schrijven.

![Augment](https://upload.wikimedia.org/wikipedia/commons/2/2b/Augment_logo.png)

Augment is een augmented reality SaaS-platform waarmee gebruikers hun producten in 3D kunnen visualiseren in een echte omgeving en in realtime via tablets of smartphones. De software kan worden gebruikt voor detailhandel, e-commerce, architectuur en andere doeleinden. Zoals men kan verwachten is deze software betalend & dus minder interessant als student.


### Coding?

Natuurlijk kan de link met coderen niet ontbreken. Hierbij zal ik gebruik maken van Snapchat's "Lens Studio" om de animatie van een 3D Blender model te voorzien binnen de Augmented Reality interface van je Snapchat applicatie.


![Lens Studio](https://www.roadtovr.com/wp-content/uploads/2017/12/snapchat-lens-studio.jpg)

Lens Studio biedt een script-engine aan voor interactieve ervaringen te creëren. Met scripts kunnen de filters reageren op aanraakinvoer, animatie en audio afspelen, scèneobjecten wijzigen en meer. 

Voorbeeld : animeren van een object dat op en neer botst.
```
// Bounce.js
// Event: Frame Updated
// Properties:
//@input float speed = 1.0 {"widget": "slider", "min": 0, "max": 10.0, "step": 0.01}
//@input float range = 10.0 {"widget": "slider", "min": 0, "max": 30.0, "step": 0.01}
var newY = Math.sin(getTime() * script.speed) * script.range;
script.getSceneObject().getTransform().setLocalPosition(new vec3(0, newY, 0));

```

### Uitwerking

De uitwerking van de code ziet er als volgt uit : 

![Codevoorbeeld](https://storage.googleapis.com/snapchat-lens-assets/f1a09194-f02d-43ed-92b8-62e843179ff0/lensStudio/Guides/img/scripting_example_preview.gif)

### Toepassing op 3D modellen

Als toepassing zal ik een codevoorbeeld schrijven om 3D modellen te kunnen manipuleren via de touch interface van Snapchat. Hiermee kan de gebruiker objecten scalen & draaien, hetgeen men ook kan bereiken binnen Blender.


Verwachte uitwerking : 

![Codevoorbeeld](https://storage.googleapis.com/snapchat-lens-assets/f1a09194-f02d-43ed-92b8-62e843179ff0/lensStudio/Guides/img/3d_object_manipulation_type_scale.gif)

