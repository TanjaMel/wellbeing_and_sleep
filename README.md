# Hyvinvointi ja unianalyysi

## Johdanto
Uni, stressi ja elämäntavat vaikuttavat sekä fyysiseen että henkiseen terveyteen. Tämän projektin tavoitteena on tutkia, miten nämä tekijät ovat yhteydessä toisiinsa ja voivatko ne auttaa tunnistamaan hyvinvointiriskejä.

## Tutkimuskysymykset

1. Mitkä elämäntapatekijät ovat vahvimmin yhteydessä stressitasoon?
2. Onko unihäiriöistä kärsivillä todennäköisemmin korkeampi stressitaso?
3. Näkyvätkö eri ammateissa erilaiset hyvinvointimallit?
4. Liittyykö korkeampi syke huonompaan unen laatuun?
5. Eroavatko yli 35-vuotiaiden stressi- ja aktiivisuusmallit muista?
6. Liittyvätkö epäterveelliset BMI-luokat sykkeen eroihin?
7. Miten unen kesto vaihtelee aineiston henkilöiden välillä?
8. Onko sykkeen jakaumassa merkittäviä eroja miesten ja naisten välillä?
9. Voivatko uni- ja elämäntapadata auttaa tunnistamaan epätavallisia hyvinvointimalleja?

## Hypoteesien tarkistus

1. Vähemmän askelia = korkeampi stressi. 
    Korrelaatio 0.19 - yhteys liian heikko. **Ei tuettu.**
2. Yli 35-vuotiailla alhaisempi aktiivisuus > korkeampi stressi.
    Hajontakuvio ei näytä selkeää trendiä. **Ei tuettu.**
3. BMI-luokka vaikuttaa sykkeeseen.
    Obese-ryhmän syke (84) on selvästi korkeampi kuin Normal-ryhmän (69). **Tuettu**
4. Joillakin ammateilla korkeampi stressi ja huonompi uni.
    Sales Representative - ammatin stressitaso (8) on lähes kaksinkertainen Engineer-ammattiin (4) verrattuna **Tuettu**
5. Miesten ja naisten syke eroaa toisistaan.
    Miesten keskisyke (~71) on hieman korkeampi kuin naisten (~69), mutta naisten sykkeen vaihteluväli on huomattavasti suurempi (65–84). **Osittain tuettu**

## Aineiston kuvaus

Tässä projektissa käytin Sleep Health and Lifestyle Dataset aineistoa Kagglesta. 
Se sisältää 374 havaintoa ja 13 saraketta, jotka kuvaavat unitottumuksia, elämäntapoja ja perusterveydentilan indikaattoreita eri ammateissa toimivilla henkilöillä.
Sarakkeet sisältävät demografisia tietoja (sukupuoli, ikä, ammatti), uneen liittyviä muuttujia (unen kesto, unen laatu, unihäiriö) sekä elämäntapa ja terveysindikaattoreita (fyysisen aktiivisuuden taso, päivittäiset askeleet, stressitaso, BMI-luokka, verenpaine ja syke).

## Eettiset näkökulmat ja tietosuoja

Tämä analyysi on tehty terveydenhuollon ennaltaehkäisevän työn tueksi. Tavoitteena on tunnistaa hyvinvointiriskejä elämäntapadatan avulla ennen kuin ongelmat pahenevat.

Hyvinvointidata sisältää arkaluonteista terveystietoa, joten sen käsittelyssä tulee huomioida tietosuoja ja GDPR.
Mallia ei käytetä lääketieteelliseen diagnosointiin, vaan hyvinvoinnin riskitekijöiden tunnistamiseen.
Anomaly detection voi tuottaa virheellisiä hälytyksiä, joten tuloksia tulisi käyttää asiantuntijan tukena eikä automaattisena päätöksentekona.

Aineiston mahdolliset vinoumat voivat vaikuttaa mallin tuloksiin.