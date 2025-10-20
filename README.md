# Ostokseni

Progressive Web App (PWA) ostoslistojen ja päiväsuunnitelmien hallintaan. 
Katso myös sivusto: https://seijalauronen.github.io/

## Ominaisuudet

- Tuotteiden hallinta kategorioittain 
- Ostoslistat tuotteille määrineen ja yksikköineen
- Päiväsuunnitelmat aterioille ja tuotteille
- Tuoteluokittelu (esim. proteiinit, hiilihydraatit jne.)
- Värikoodaus tuotteille
- Offline-käyttö mahdollista PWA-ominaisuuden ansiosta
- Tietojen vienti/tuonti JSON-muodossa
- Responsiiivinen käyttöliittymä mobiili- ja työpöytäkäyttöön

## Teknologiat

- React 18.3
- Styled Components
- IndexedDB tietokanta (idb-kirjasto)
- Service Worker PWA-toiminnallisuudelle
- Hello-pangea/dnd drag & drop -toiminnallisuuteen
- FontAwesome ikonit
- React Device Detect laitetunnistukseen

## Kehitys

1. Kloonaa repositorio
2. Asenna riippuvuudet:
```bash
npm install
```
3. Käynnistä kehitysympäristö:
```bash 
npm start
```

## Tuotantoversion luonti

Luo tuotantoversio:
```bash
npm run build
```

## Testaus

Suorita testit:
```bash
npm test
```

## Arkkitehtuuri

- React komponentit src/components hakemistossa
- Näkymät src/views hakemistossa
- Tietokantaoperaatiot src/dbUtils.js
- Kontrollerikerros src/controller.js
- Context tilanhallintaan:
  - SettingsContext
  - ColorContext 
  - ProductClassContext

## Asennus

Sovellus on asennettavissa PWA:na selaimesta "Asenna" -toiminnolla. Tiedot tallentuvat selaimen IndexedDB:hen.

## Käyttöönotto

1. Ensimmäisellä käynnistyksellä voit ladata esimerkkiaineiston
2. Lisää omat kategoriat ja tuotteet
3. Luo ostoslistoja valitsemalla tuotteita ostoskoriin
4. Voit ottaa käyttöön päiväsuunnittelun asetuksista


## Tekijänoikeudet ja käyttöehdot

Copyright © 2025 Seija Lauronen. Kaikki oikeudet pidätetään.

### Sallittu käyttö:
- Koodin lataaminen ja tutkiminen opiskelutarkoituksessa
- Sovelluksen testaaminen omalla koneella
- Koodin muokkaaminen omaan henkilökohtaiseen käyttöön

### Kielletty käyttö:
- Koodin tai sen osien kaupallinen käyttö
- Koodin jakaminen tai levittäminen eteenpäin
- Sovelluksen julkaiseminen missään muodossa
- Koodin käyttö osana muita projekteja ilman erillistä lupaa

Tämä projekti on henkilökohtainen oppimisprojekti. Jos haluat käyttää koodia muihin tarkoituksiin, ota yhteyttä tekijään luvan saamiseksi.