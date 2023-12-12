# Sentimentanalys med IMDb-dataset

Detta projekt utför sentimentanalys på recensioner från IMDb-datasetet. Syftet är att bygga och utvärdera maskininlärningsmodeller för att klassificera recensioner som antingen positiva eller negativa baserat på textinnehållet.

## Steg 1: Datainsamling

Datasetet laddas in från filen 'IMDB Dataset.csv'. En andel av datamängden kan slumpmässigt väljas för att förbättra hanterbarheten och minska träningskostnaderna.

## Steg 2: Utforska och förbereda data

- Kontrollera nollvärden och statistik för datasetet.
- Visualisera klassbalansen mellan positiva och negativa recensioner.
- Dela upp datasetet i positiva och negativa recensioner.
- Förbered texten genom att rensa bort specialtecken, omvandla till små bokstäver, ta bort stoppord och tokenisera.

## Steg 3: Analys av mest använda ord

- Skapa och skriv ut listor över de mest förekommande orden i både positiva och negativa recensioner.
- Skapa histogram för de mest använda orden i positiva och negativa recensioner.
- Skapa och visa ordmoln för både positiva och negativa recensioner.

## Steg 4: Modellträning och utvärdering

- Dela upp datasetet i tränings- och testdata.
- Skapa TF-IDF-vektorer för texten.
- Skala vektorerna med MaxAbs-scaling.
- Träna modeller: Logistisk regression, Multinomial Naive Bayes och Linear Support Vector Classifier.
- Utvärdera modellerna med noggrannhet och classification report.

## Steg 5: Använda modellerna för förutsägelser

Gör förutsägelser på nya recensioner för att bedöma deras sentiment.

## Viktiga bibliotek och verktyg:

- Pandas: För datahantering och analys.
- Matplotlib och WordCloud: För visualisering av data.
- NLTK: För textförberedelse och tokenisering.
- Scikit-learn: För maskininlärningsmodeller och utvärdering.
- Tabulate: För att presentera mest använda ord i tabellformat.

## Användning av kod

För att använda koden, installera nödvändiga bibliotek med `pip install -r requirements.txt` och kör kodcellerna i en Jupyter Notebook eller liknande miljö. Se till att ha 'IMDB Dataset.csv' i en 'data'-mapp i samma katalog som notebooken. Anpassa kod efter behov och utforska olika modeller för bästa prestanda.

**Observera:** Projektet innefattar maskininlärningsmodeller som kräver träningsdata. Prestanda kan variera beroende på dataset och experiment.
