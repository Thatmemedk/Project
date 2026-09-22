## Mål
Analysera jobbannonser med Python för att undersöka vilka teknologier som efterfrågas i roller med koppling till AI-utveckling.

## Metod
JobTech API används som extern datakälla. Sökningar görs på flera AI-relaterade sökord ("AI-utvecklare", "maskininlärning", "data scientist", "AI"). Relevanta fält struktureras med hjälp av klasserna `JobAnnons` (basklass) och `AIJobbannons` (barnklass, ärver från `JobAnnons` och lägger till en lista med hittade teknologier). Resultatet sparas i `jobbdata.csv` med standardbiblioteket `csv`. Därefter används keyword-matching för att räkna förekomsten av utvalda teknologier (Python, Java, AWS, Azure, Docker, SQL, JavaScript, Kubernetes, Machine Learning, AI) och Matplotlib används för att visualisera resultatet som ett stapeldiagram. API-anrop och filskrivning skyddas med `try/except` för att hantera nätverksfel respektive filfel.

## Resultat
- De 5 vanligaste teknologierna och antal förekomster:
  1. AI
  2. Python
  3. Azure
  4. Machine Learning
  5. SQL

## Analys
Resultatet kopplas till AI-utvecklarrollen genom att visa vilka tekniska kompetenser som förekommer i det analyserade urvalet av jobbannonser. Slutsatserna ska begränsas till det insamlade urvalet, eftersom det bara är ett litet stickprov av det svenska jobbmarknadsutbudet och inte en fullständig kartläggning av branschen.

## Certifikat
Utifrån de teknologier som ofta efterfrågas i AI-relaterade roller (moln, data, Python) är följande certifieringar särskilt relevanta för en AI-utvecklare:

- **AWS Certified Machine Learning – Specialty / AWS Certified Cloud Practitioner** – visar kompetens inom molndrift och ML-tjänster på AWS, vilket är vanligt förekommande i svenska jobbannonser.
- **Microsoft Certified: Azure AI Engineer Associate** – relevant eftersom många svenska företag använder Microsoft Azure för AI- och datalösningar.
- **Databricks Certified Data Engineer Associate** – relevant för hantering och bearbetning av stora datamängder, vilket är en central del av AI-utvecklarrollen.

Dessa certifieringar valdes eftersom de täcker moln (AWS/Azure), som återkommer bland de vanligaste teknologierna i analysen, samt datahantering (Databricks), vilket är en grundpelare i AI-utveckling.

## Reflektion

### Vad gick bra?
API-anropet fungerade bra och jag kunde hämta fem jobbannonser från JobTech. Jag kunde också se och kontrollera informationen i annonserna.

### Vad var svårt?
Det var svårt att förstå den stora mängden information som finns i JSON-datan och vilka delar som är viktigast för analysen.

### Vad skulle jag göra annorlunda?
Jag skulle hämta fler jobbannonser för att få ett större underlag. Jag skulle också rensa och strukturera datan bättre innan jag börjar analysera den.

## GitHub
Repository: https://github.com/Thatmemedk/Project

## Installation
`pip install -r requirements.txt`

Öppna sedan `jobbannons_analys_UPPDATERAD.ipynb` i Jupyter, VS Code eller Google Colab och kör cellerna uppifrån och ned.