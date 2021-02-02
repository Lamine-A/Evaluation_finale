
# ![alt tag](https://t3.ldh.be/vCLkhdTglDrD-n_qq_EMNt4PQ3c=/0x0:940x470/940x470/5e3fb307d8ad5878d86262ae.jpg)
# Sommaire
1. [Introduction](#introduction)
2. [Jeu de données sur les "Accidents corporels de la circulation millésimé (2012/2017)"](#paragraph1)
    1. [Représentation des la gravité des accidents par année](#subparagraph1)
    2. [Repartition](#subparagraph2)
    3. [localisation la plus meurtriere](#subparagraph4)
    4. [Comparaison des victimes en fonction de leur sexe](#subparagraph5)
    5. [Carte](#subparagraph6)
3. [Traitement du jeu des données des accidents sur l'année 2019 sur Openrefine](#paragraph2)
    1. [Présentaion](#subparagraph1)
    2. [Fichier Json des traitements](#subparagraph2)
    
4. [Utilistaion de wikidata pour analyser les accidents d'avions dans le monde ](#paragraph3)
    1. [Première requête: les accidents d'avion dans le monde](#subparagraph1)
    2. [Deuxième requête: Carte mondiale des accidents d'avions dans le monde](#subparagraph2)
5. [Conculsion](#paragraph4)

## Introduction <a name="Introduction"></a>
Some introduction text, formatted in heading 2 style

##  Jeu de données sur les "Accidents corporels de la circulation millésimé" <a name="paragraph1"></a>
<iframe src="https://data.opendatasoft.com/explore/embed/dataset/accidents-corporels-de-la-circulation-millesime@public/table/?disjunctive.com_name&disjunctive.dep_code&disjunctive.dep_name&disjunctive.epci_code&disjunctive.epci_name&disjunctive.reg_code&disjunctive.reg_name&disjunctive.com_code&static=false&datasetcard=false" width="860" height="500" frameborder="30"></iframe>

### Représentation de la gravité des accidents par année <a name="subparagraph1"></a>
<iframe src="https://data.opendatasoft.com/explore/embed/dataset/accidents-corporels-de-la-circulation-millesime@public/analyze/?disjunctive.com_name&disjunctive.dep_code&disjunctive.dep_name&disjunctive.epci_code&disjunctive.epci_name&disjunctive.reg_code&disjunctive.reg_name&disjunctive.com_code&dataChart=eyJxdWVyaWVzIjpbeyJjaGFydHMiOlt7InR5cGUiOiJjb2x1bW4iLCJmdW5jIjoiQ09VTlQiLCJ5QXhpcyI6ImxhcnJvdXQiLCJzY2llbnRpZmljRGlzcGxheSI6dHJ1ZSwiY29sb3IiOiJyYW5nZS1jdXN0b20ifV0sInhBeGlzIjoiZGF0ZSIsIm1heHBvaW50cyI6IiIsInRpbWVzY2FsZSI6InllYXIiLCJzb3J0IjoiIiwiY29uZmlnIjp7ImRhdGFzZXQiOiJhY2NpZGVudHMtY29ycG9yZWxzLWRlLWxhLWNpcmN1bGF0aW9uLW1pbGxlc2ltZUBwdWJsaWMiLCJvcHRpb25zIjp7ImRpc2p1bmN0aXZlLmNvbV9uYW1lIjp0cnVlLCJkaXNqdW5jdGl2ZS5kZXBfY29kZSI6dHJ1ZSwiZGlzanVuY3RpdmUuZGVwX25hbWUiOnRydWUsImRpc2p1bmN0aXZlLmVwY2lfY29kZSI6dHJ1ZSwiZGlzanVuY3RpdmUuZXBjaV9uYW1lIjp0cnVlLCJkaXNqdW5jdGl2ZS5yZWdfY29kZSI6dHJ1ZSwiZGlzanVuY3RpdmUucmVnX25hbWUiOnRydWUsImRpc2p1bmN0aXZlLmNvbV9jb2RlIjp0cnVlfX0sInNlcmllc0JyZWFrZG93biI6ImdyYXYifV0sImRpc3BsYXlMZWdlbmQiOnRydWUsImFsaWduTW9udGgiOnRydWV9&static=false&datasetcard=false" width="860" height="500" frameborder="60"></iframe>
### Repartition <a name="subparagraph2"></a>
<iframe src="https://data.opendatasoft.com/explore/embed/dataset/accidents-corporels-de-la-circulation-millesime@public/analyze/?disjunctive.com_name&disjunctive.dep_code&disjunctive.dep_name&disjunctive.epci_code&disjunctive.epci_name&disjunctive.reg_code&disjunctive.reg_name&disjunctive.com_code&location=3,18.51908,-3.0018&basemap=jawg.streets&dataChart=eyJxdWVyaWVzIjpbeyJjaGFydHMiOlt7InR5cGUiOiJwaWUiLCJmdW5jIjoiQ09VTlQiLCJ5QXhpcyI6ImxhcnJvdXQiLCJzY2llbnRpZmljRGlzcGxheSI6dHJ1ZSwiY29sb3IiOiJyYW5nZS1jdXN0b20iLCJwb3NpdGlvbiI6ImNlbnRlciJ9XSwieEF4aXMiOiJncmF2IiwibWF4cG9pbnRzIjoxMDAsInRpbWVzY2FsZSI6IiIsInNvcnQiOiJzZXJpZTEtMSIsImNvbmZpZyI6eyJkYXRhc2V0IjoiYWNjaWRlbnRzLWNvcnBvcmVscy1kZS1sYS1jaXJjdWxhdGlvbi1taWxsZXNpbWVAcHVibGljIiwib3B0aW9ucyI6eyJkaXNqdW5jdGl2ZS5jb21fbmFtZSI6dHJ1ZSwiZGlzanVuY3RpdmUuZGVwX2NvZGUiOnRydWUsImRpc2p1bmN0aXZlLmRlcF9uYW1lIjp0cnVlLCJkaXNqdW5jdGl2ZS5lcGNpX2NvZGUiOnRydWUsImRpc2p1bmN0aXZlLmVwY2lfbmFtZSI6dHJ1ZSwiZGlzanVuY3RpdmUucmVnX2NvZGUiOnRydWUsImRpc2p1bmN0aXZlLnJlZ19uYW1lIjp0cnVlLCJkaXNqdW5jdGl2ZS5jb21fY29kZSI6dHJ1ZX19LCJzZXJpZXNCcmVha2Rvd24iOiIiLCJzZXJpZXNCcmVha2Rvd25UaW1lc2NhbGUiOiIifV0sImRpc3BsYXlMZWdlbmQiOnRydWUsImFsaWduTW9udGgiOnRydWUsInRpbWVzY2FsZSI6IiJ9&static=false&datasetcard=false" width="860" height="500" frameborder="10"></iframe>
### localisation la plus meurtriere <a name="subparagraph3"></a>
<iframe src="https://data.opendatasoft.com/explore/embed/dataset/accidents-corporels-de-la-circulation-millesime@public/analyze/?disjunctive.com_name&disjunctive.dep_code&disjunctive.dep_name&disjunctive.epci_code&disjunctive.epci_name&disjunctive.reg_code&disjunctive.reg_name&disjunctive.com_code&location=3,18.51908,-3.0018&basemap=jawg.streets&dataChart=eyJxdWVyaWVzIjpbeyJjaGFydHMiOlt7InR5cGUiOiJjb2x1bW4iLCJmdW5jIjoiQ09VTlQiLCJ5QXhpcyI6ImxhcnJvdXQiLCJzY2llbnRpZmljRGlzcGxheSI6dHJ1ZSwiY29sb3IiOiJyYW5nZS1jdXN0b20iLCJwb3NpdGlvbiI6ImNlbnRlciJ9XSwieEF4aXMiOiJhZ2ciLCJtYXhwb2ludHMiOjIwMCwidGltZXNjYWxlIjoiIiwic29ydCI6IiIsImNvbmZpZyI6eyJkYXRhc2V0IjoiYWNjaWRlbnRzLWNvcnBvcmVscy1kZS1sYS1jaXJjdWxhdGlvbi1taWxsZXNpbWVAcHVibGljIiwib3B0aW9ucyI6eyJkaXNqdW5jdGl2ZS5jb21fbmFtZSI6dHJ1ZSwiZGlzanVuY3RpdmUuZGVwX2NvZGUiOnRydWUsImRpc2p1bmN0aXZlLmRlcF9uYW1lIjp0cnVlLCJkaXNqdW5jdGl2ZS5lcGNpX2NvZGUiOnRydWUsImRpc2p1bmN0aXZlLmVwY2lfbmFtZSI6dHJ1ZSwiZGlzanVuY3RpdmUucmVnX2NvZGUiOnRydWUsImRpc2p1bmN0aXZlLnJlZ19uYW1lIjp0cnVlLCJkaXNqdW5jdGl2ZS5jb21fY29kZSI6dHJ1ZX19LCJzZXJpZXNCcmVha2Rvd24iOiJncmF2Iiwic2VyaWVzQnJlYWtkb3duVGltZXNjYWxlIjoiIn1dLCJkaXNwbGF5TGVnZW5kIjp0cnVlLCJhbGlnbk1vbnRoIjp0cnVlLCJ0aW1lc2NhbGUiOiIifQ%3D%3D&static=false&datasetcard=false" width="860" height="500" frameborder="10"></iframe>
### Comparaison des victimes en fonction de leur sexe <a name="subparagraph4"></a>
<iframe src="https://data.opendatasoft.com/explore/embed/dataset/accidents-corporels-de-la-circulation-millesime@public/analyze/?disjunctive.com_name&disjunctive.dep_code&disjunctive.dep_name&disjunctive.epci_code&disjunctive.epci_name&disjunctive.reg_code&disjunctive.reg_name&disjunctive.com_code&location=3,18.51908,-3.0018&basemap=jawg.streets&dataChart=eyJxdWVyaWVzIjpbeyJjaGFydHMiOlt7InR5cGUiOiJjb2x1bW4iLCJmdW5jIjoiQ09VTlQiLCJ5QXhpcyI6ImxhcnJvdXQiLCJzY2llbnRpZmljRGlzcGxheSI6dHJ1ZSwiY29sb3IiOiJyYW5nZS1jdXN0b20iLCJwb3NpdGlvbiI6ImNlbnRlciJ9XSwieEF4aXMiOiJncmF2IiwibWF4cG9pbnRzIjoyMDAsInRpbWVzY2FsZSI6IiIsInNvcnQiOiIiLCJjb25maWciOnsiZGF0YXNldCI6ImFjY2lkZW50cy1jb3Jwb3JlbHMtZGUtbGEtY2lyY3VsYXRpb24tbWlsbGVzaW1lQHB1YmxpYyIsIm9wdGlvbnMiOnsiZGlzanVuY3RpdmUuY29tX25hbWUiOnRydWUsImRpc2p1bmN0aXZlLmRlcF9jb2RlIjp0cnVlLCJkaXNqdW5jdGl2ZS5kZXBfbmFtZSI6dHJ1ZSwiZGlzanVuY3RpdmUuZXBjaV9jb2RlIjp0cnVlLCJkaXNqdW5jdGl2ZS5lcGNpX25hbWUiOnRydWUsImRpc2p1bmN0aXZlLnJlZ19jb2RlIjp0cnVlLCJkaXNqdW5jdGl2ZS5yZWdfbmFtZSI6dHJ1ZSwiZGlzanVuY3RpdmUuY29tX2NvZGUiOnRydWV9fSwic2VyaWVzQnJlYWtkb3duIjoibHVtIiwic2VyaWVzQnJlYWtkb3duVGltZXNjYWxlIjoiIn1dLCJkaXNwbGF5TGVnZW5kIjp0cnVlLCJhbGlnbk1vbnRoIjp0cnVlLCJ0aW1lc2NhbGUiOiIifQ%3D%3D&static=false&datasetcard=false" width="860" height="500" frameborder="10"></iframe> 
### cause eclairage <a name="subparagraph5"></a>
<iframe src="https://data.opendatasoft.com/explore/embed/dataset/accidents-corporels-de-la-circulation-millesime@public/analyze/?disjunctive.com_name&disjunctive.dep_code&disjunctive.dep_name&disjunctive.epci_code&disjunctive.epci_name&disjunctive.reg_code&disjunctive.reg_name&disjunctive.com_code&dataChart=eyJxdWVyaWVzIjpbeyJjaGFydHMiOlt7InR5cGUiOiJjb2x1bW4iLCJmdW5jIjoiQ09VTlQiLCJ5QXhpcyI6ImxhcnJvdXQiLCJzY2llbnRpZmljRGlzcGxheSI6dHJ1ZSwiY29sb3IiOiJyYW5nZS1jdXN0b20ifV0sInhBeGlzIjoiZ3JhdiIsIm1heHBvaW50cyI6IiIsInRpbWVzY2FsZSI6IiIsInNvcnQiOiIiLCJjb25maWciOnsiZGF0YXNldCI6ImFjY2lkZW50cy1jb3Jwb3JlbHMtZGUtbGEtY2lyY3VsYXRpb24tbWlsbGVzaW1lQHB1YmxpYyIsIm9wdGlvbnMiOnsiZGlzanVuY3RpdmUuY29tX25hbWUiOnRydWUsImRpc2p1bmN0aXZlLmRlcF9jb2RlIjp0cnVlLCJkaXNqdW5jdGl2ZS5kZXBfbmFtZSI6dHJ1ZSwiZGlzanVuY3RpdmUuZXBjaV9jb2RlIjp0cnVlLCJkaXNqdW5jdGl2ZS5lcGNpX25hbWUiOnRydWUsImRpc2p1bmN0aXZlLnJlZ19jb2RlIjp0cnVlLCJkaXNqdW5jdGl2ZS5yZWdfbmFtZSI6dHJ1ZSwiZGlzanVuY3RpdmUuY29tX2NvZGUiOnRydWV9fSwic2VyaWVzQnJlYWtkb3duIjoic2V4ZSJ9XSwiZGlzcGxheUxlZ2VuZCI6dHJ1ZSwiYWxpZ25Nb250aCI6dHJ1ZSwidGltZXNjYWxlIjoiIn0%3D&static=false&datasetcard=false" width="800" height="600" frameborder="0"></iframe>
### Carte <a name="subparagraph6"></a>
<iframe frameborder="0" width="860" height="700" src="https://data.opendatasoft.com/map/embed/accidents/?&static=true&scrollWheelZoom=true"></iframe>

## Traitement du jeu donnée des accidents sur l'année 2019 <a name="paragraph2"></a>
### Présentation <a name="subparagraph1"></a>
### Fichier Json des traitements <a name="subparagraph2"></a>

## Utilistaion de wikidata pour analyser les accidents d'avions dans le monde <a name="paragraph3"></a>)
### Première requête: les accidents d'avion dans le monde <a name="subparagraph1"></a>
### Deuxième requête: Carte mondiale des accidents d'avions dans le monde <a name="subparagraph2"></a>
````sparql
#Lieux des accidents d’avions
SELECT ?label ?coord ?place
WHERE
{
   ?subj wdt:P31 wd:Q744913  .
   ?subj wdt:P625 ?coord .
   ?subj rdfs:label ?label filter (lang(?label) = "fr")
}
````
### Résultat
<iframe style="width: 60vw; height: 30vh; border: none;" src="https://query.wikidata.org/embed.html#%23Lieux%20des%20accidents%20d%E2%80%99avions%0ASELECT%20%3Flabel%20%3Fcoord%20%3Fplace%0AWHERE%0A%7B%0A%20%20%20%3Fsubj%20wdt%3AP31%20wd%3AQ744913%20%20.%0A%20%20%20%3Fsubj%20wdt%3AP625%20%3Fcoord%20.%0A%20%20%20%3Fsubj%20rdfs%3Alabel%20%3Flabel%20filter%20(lang(%3Flabel)%20%3D%20%22fr%22)%0A%7D" referrerpolicy="origin" sandbox="allow-scripts allow-same-origin allow-popups"></iframe>

## Conculsion <a name="paragraph4"></a>


