# Hyvinvointi ja unianalyysi

## Johdanto

Uni, stressi ja elämäntavat vaikuttavat merkittävästi sekä fyysiseen että henkiseen hyvinvointiin. Tämän projektin tavoitteena oli analysoida hyvinvointiin liittyviä yhteyksiä data-analytiikan ja koneoppimisen avulla sekä tutkia, voidaanko hyvinvointidatasta tunnistaa epätavallisia hyvinvointiprofiileja.

Projektissa hyödynnettiin Exploratory Data Analysis (EDA)-menetelmiä, korrelaatioanalyysiä, feature selection -vaihetta, anomaly detection-mallia sekä supervised learning-analyysiä cross-validation-menetelmällä.


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

## Aineiston kuvaus

Projektissa käytettiin Sleep Health and Lifestyle Dataset-aineistoa Kagglesta.

Aineisto sisältää 374 havaintoa ja useita hyvinvointiin liittyviä muuttujia:
- ikä
- sukupuoli
- ammatti
- unen kesto
- unen laatu
- stressitaso
- fyysinen aktiivisuus
- päivittäiset askeleet
- BMI-luokka
- syke
- verenpaine
- unihäiriöt

Analyysissä käytettiin sekä alkuperäistä korrelaatioheatmapia että reduced correlation heatmap -versiota, jossa erittäin vahvasti korreloivia muuttujia poistettiin feature selection -vaiheessa multicollinearity-ilmiön vähentämiseksi.

## Käytetyt menetelmät

Projektissa käytettiin:
- Exploratory Data Analysis (EDA)
- korrelaatioanalyysiä
- reduced correlation heatmap -analyysiä
- feature selection -vaihetta
- anomaly detection -analyysiä Isolation Forest -algoritmilla
- supervised learning -analyysiä
- cross-validation -menetelmää
- visualisointeja Matplotlib- ja Seaborn-kirjastoilla

Isolation Forest-mallia käytettiin epätavallisten hyvinvointiprofiilien tunnistamiseen. Mallin arviointi perustui anomaly count-analyysiin, visualisointeihin sekä poikkeavien havaintojen tulkintaan, koska kyseessä oli unsupervised learning-menetelmä.

Supervised learning-vaiheessa käytettiin 5-fold cross-validation -menetelmää mallin vakauden arviointiin.

