# Zeilgids Dodekanesos & Cycladen (Oktober • 35ft • Basis: Kos)

Een statische, interactieve schippersgids voor een zeiltocht met een 35-voets zeiljacht in oktober, vertrekkend vanuit Kos Harbor (Archon Yachting).

## Status

Prototype: de repository bestaat uit één enkel HTML-bestand (`index.html`) zonder package manager, build-proces of test-suite. De git-historie bevat tot nu toe alleen het hernoemen van dat bestand.

## Waarom

Tijdens een najaarstocht door de Dodekanesos en Cycladen moet een schipper snel kunnen schakelen tussen windinformatie, beschutting van havens, cultuur, fauna en afstanden. Deze pagina bundelt die informatie in één doorzoekbaar dashboard, zodat je niet tussen meerdere bronnen hoeft te wisselen. Alle inhoud is toegespitst op een specifieke route met Kos als thuisbasis en een kruissnelheid van 5,5 knopen.

## Snel starten

Er is geen installatie nodig: het bestand gebruikt Tailwind CSS via een CDN-script en bevat verder alleen platte HTML en JavaScript.

Open het bestand direct in je browser:

```bash
# Linux
xdg-open index.html

# Windows (Git Bash)
start index.html
```

Of serveer het lokaal (handig als je browser lokale bestandstoegang beperkt):

```bash
python3 -m http.server 8000
# open vervolgens http://localhost:8000 in de browser
```

## Gebruik

- **Navigatietabs**: bovenaan de pagina schakel je tussen zeven secties — Wind & Beschutting, Historie & Lokale Cultuur, Lokale Fauna, Najaarsevenementen, Zeekaartgids, Eilandfocus en Kaart & Afstanden.
- **Snel filteren**: het zoekveld boven de tabs (`quickFilter`) filtert tabelrijen en kaarten op eiland, haven of kenmerk terwijl je typt.
- **Afstands- en vaartijdcalculator**: in de tab "Kaart & Afstanden" kies je een vertrek- en aankomsthaven; de calculator berekent de afstand in zeemijlen en de geschatte vaartijd op basis van 5,5 knopen.
- **Interactieve zeekaart**: een inline SVG-kaart met havenmarkers; klik op een havenmarker voor schipperstactiek per locatie.

## Structuur

```
.
└── index.html   # Volledige applicatie: HTML-inhoud, Tailwind-configuratie en JavaScript (tabs, filter, afstandscalculator) in één bestand
```

> TODO: aanvullen — er is geen licentie- of contactinformatie in de repository aanwezig.
