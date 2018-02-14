# ShipTrack

> Shipment tracking via a tracking number. Shows the current status and the history of the whereabouts of the shipment. 
> You can send in new shipping request via the administration ui and update the status with the update status ui

try out the hosted version on heroku

![alt text](https://raw.githubusercontent.com/konstantinsteinmiller/shipment-tracking/master/images/shiptrack-search.PNG)

![alt text](https://raw.githubusercontent.com/konstantinsteinmiller/shipment-tracking/master/images/shiptrack-tracking.PNG)

![alt text](https://raw.githubusercontent.com/konstantinsteinmiller/shipment-tracking/master/images/shiptrack-update.PNG)

![alt text](https://raw.githubusercontent.com/konstantinsteinmiller/shipment-tracking/master/images/shiptrack-admin.PNG)

## Build Setup
``` bash
to launch locally follow instructions in the /backend/readme.md and the /fronend/readme.md
```

### Workflow + Architecture

![alt text](https://raw.githubusercontent.com/konstantinsteinmiller/shipment-tracking/master/images/shiptrack.jpg)

>

### Scenario

>Ausgangslage: Oma Paschulke möchte ihrem Enkel Max von Hamburg nach München einen Band aus seiner Lieblingsbuchreihe schicken. Sie möchte das Buch mit Hermes versenden. Dafür bringt sie das verpackte Buch zum Paketshop um die Ecke. Dort gibt sie es ab und erhält eine mehrstellige Sendungsnummer.
 Mit Hilfe dieser Sendungsnummer möchte sie den Weg des Paketes bequem am eigenen Computer nachvollziehen - und hier bist Du gefragt!
 
 {INPUT/REQUIREMENTS}
 
> Das ist Deine Aufgabe:
 Erstelle einen Service, der eine eindeutige Sendungsnummer generiert. Die Anzahl der Stellen ist selbst zu wählen und zu Begründen. Ein Bezug der Stellen zu Ort, Zeit und Art der Sendung ist wünschenswert. Bitte überlege, ob ggf. weitere Werte in der Sendungsnummer wieder gegeben werden können oder müssen (z.B. eine Richtung).
 Der Service bildet anhand der Sendungsverfolgungsnummer die logische Kette des Transports ab, die unterschiedliche logistische Status beinhaltet.
 Zum Beispiel: Vom Paketshop wird das Buch zu der Niederlassung Hamburg transportiert und von dort zum regionalen Verteilzentrum transportiert. Weiter geht es dann in die Niederlassung München und von dort erfolgt die Zustellung an Enkel Max.
 Wie lassen sich die verschiedenen Status am effizientesten/sinnvollsten speichern?
 Über ein kleines Frontend können Oma Paschulke und Enkel Max jederzeit Auskunft darüber bekommen, wo sich das Paket befindet (mithilfe der Sendungsnummer). Die einzelnen Transportschritte können über das Frontend nachvollzogen werden.

### Usage
> Navigation is possible by clicking the burger menu button at the top left corner.

> Before you can use the tracking feature, you have to navigate to the administration ui 
and create a new tracking number by submitting some data for shipment
select a shipment type and enter source and target adresses.
Default values are provided for the scenario.

> After creating a tracking number you can fetch the current status of the shipment by entering the
tracking number in the tracking ui.

> You can also update the tracking status manually by sending in new information by using the update shipment ui.
Changes can be seen in the tracking UI after refetching with the according tracking number.