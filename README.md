## Mål
Analysera jobbannonser med Python för att undersöka vilka teknologier som efterfrågas i roller med koppling till AI-utveckling.

## Metod
JobTech API används som extern datakälla. Relevanta fält extraheras och sparas i `jobbdata.csv`. Därefter används keyword-matching för att räkna förekomsten av utvalda teknologier och Matplotlib för visualisering. Projektet innehåller även OOP med arv och `try/except` för felhantering.

## Resultat
Fylls i efter att API-anropet har körts. Redovisa antal annonser, vanligaste teknologier och diagram.

## Branschanalys
Resultatet kopplas till AI-utvecklarrollen genom att visa vilka tekniska kompetenser som förekommer i det analyserade urvalet av jobbannonser. Slutsatserna ska begränsas till det insamlade urvalet.

## Certifikat
Relevanta certifieringsområden att undersöka är AWS, Microsoft Azure och Databricks. Beskriv i slutversionen vilka certifikat som är relevanta för AI-/molnrelaterade arbetsuppgifter och varför.

## Reflektion

## Vad gick bra?
API-anropet fungerade bra och jag kunde hämta fem jobbannonser från JobTech. Jag kunde också se och kontrollera informationen i annonserna.

## Vad var svårt?
Det var svårt att förstå den stora mängden information som finns i JSON-datan och vilka delar som är viktigast för analysen.

## Vad skulle jag göra annorlunda?
Jag skulle hämta fler jobbannonser för att få ett större underlag. Jag skulle också rensa och strukturera datan bättre innan jag börjar analysera den.

## GitHub
Repository: https://github.com/Thatmemedk/Project

## Installation
`pip install -r requirements.txt`

Öppna sedan `jobbannons_analys.ipynb` i Jupyter, VS Code eller Google Colab och kör cellerna uppifrån och ned.