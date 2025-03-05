# Fatal-Police-Shooting-in-USA_Data-Manipulation-and-Visualization
<br>

Progetto svolto in linguaggio Python, utilizzando le librerie Numpy, Pandas, Scipy, Matplotlib e Seaborn, basato sulla Data Cleaning, Manipulation e Visualization di vari dataset.

<br>
<br>

## Discovery

<br>

### PROBLEMI :

La storia americana è stata caratterizzata da una forte componente razzista, ad esempio fino agli anni '60 gli afroamericani sono stati costretti a vivere separatamente dai bianchi, senza alcun diritto di voto.
La forte militarizzazione delle forze di polizia e la demonizzazione delle minoranze e delle classi sociali più svantaggiate, spesso associate alla criminalità, ha caratterizzato lo sviluppo di comportamenti estremamente violenti da parte degli ufficiali nei confronti dei cittadini, portando in molte occasioni alla morte degli stessi.

<br>

### OBIETTIVI :

Comprendere in quali anni ed in quali stati si è verificato un picco di casi di police brutality.
Evidenziare se il contesto sociale ed etnico di appartenenza delle vittime influenzi i casi di morte per arma da fuoco risalenti alle forze di polizia.
Analizzare i vari dipartimenti di polizia americani in base ai casi di morte per arma da fuoco in cui sono coinvolti.
(in questa EDA il termine "razza" verrà utilizzato facendo riferimento alla traduzione italiana della parola inglese "race", ossia come costrutto sociale)

<br>

## Data Selection
Le fonti scelte per questa EDA sono:

- fpsd: "Fatal Police Shooting Data" dataset sui casi di omicidio per arma da fuoco registrati dal Washington Post dal 2015 al 2024 [link](https://github.com/washingtonpost/data-police-shootings/blob/master/v2/fatal-police-shootings-data.csv)

- police_ag: "Fatal Police Shooting agencies", dataset sui dipartimenti di polizia statunitensi [link](https://github.com/washingtonpost/data-police-shootings/blob/master/v2/fatal-police-shootings-agencies.csv)

- uninsured_rate: "Uninsured people in USA 2015-2023", percentuale di cittadini senza assicurazione sanitaria per stato dal 2015 al 2023 [link](https://data.census.gov/table/ACSST1Y2023.S2701t=Health%20Insurance&g=010XX00US$0400000&moe=false&tp=false)

- poverty_rate: "USA perc below poverty 2015-2023", percentuale di persone sotto la soglia di povertà per stato dal 2015 al 2023 [link](https://data.census.gov/table/ACSST1Y2023.S1701?t=Poverty&g=010XX00US$0400000)

- education_rate: "USA perc over 25 completed H-school 2015-2023", percentuale di completamento delle High School da 25 anni in su per stato dal 2015 al 2023 [link](https://data.census.gov/table/ACSST1Y2023.S1501?t=Educational%20Attainment&g=010XX00US$0400000&moe=false)

- usa_share: "USA sharerace 2015-2023" divisone della popolazione in gruppi etnici negli Stati Uniti dal 2015 al 2023 [link](https://data.census.gov/table/ACSDP1Y2015.DP05?q=Hispanic%20or%20Latino&hidePreview=false)

- usa_states_share: "USA states share race 2015-2023", divisone della popolazione in razze nei singoli stati degli USA dal 2015 al 2023 [link](https://data.census.gov/table/ACSDP1Y2023.DP05q=Hispanic%20or%20Latino&g=010XX00US$0400000&moe=false&tp=false)

- states_population: "USA states population 2015-2023", la popolazione degli USA per stato [link 1](https://www.census.gov/data/datasets/time-series/demo/popest/2010s-state-total.html#par_textimage_500989927) , [link 2](https://www.census.gov/data/tables/time-series/demo/popest/2020s-state-total.html)

- states_abb: "USA states abbreviation", le sigle degli stati negli USA associate ai nomi [link](https://www.kaggle.com/datasets/doyouevendata/state-abbreviations)

- usa_map: mappa degli USA per creare grafici attraverso Geopandas [link](https://hub.arcgis.com/datasets/1b02c87f62d24508970dc1a6df80c98e/explore?location=39.084773%2C-106.619592%2C3.74)

<br>
<br>
