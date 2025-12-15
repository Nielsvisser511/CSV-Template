# Exact Online Grootboekrekeningen Import Template

Excel template voor het importeren van grootboekrekeningen (general ledger accounts) in Exact Online via XML.

## 📋 Overzicht

Deze template maakt het eenvoudig om grootboekrekeningen te importeren in Exact Online. Vul simpelweg de gegevens in Excel in en gebruik de ingebouwde macro om een XML-bestand te genereren dat direct in Exact Online geïmporteerd kan worden.

## ✨ Features

- ✅ Voorgeformatteerde Excel template met alle benodigde velden
- ✅ VBA macro voor automatische XML export
- ✅ Data validatie met dropdowns voor gemakkelijke invoer
- ✅ Voorbeelddata met typische Nederlandse rekeningen
- ✅ Instructies binnen Excel
- ✅ Klaar voor directe import in Exact Online

## 🚀 Snel Starten

1. Download `Grootboekrekeningen_Import_Template.xlsm`
2. Open het bestand in Excel
3. Schakel macro's in als gevraagd
4. Vul je grootboekrekeningen in (of pas de voorbeelddata aan)
5. Klik op de knop "Export naar XML" of druk op `Alt + F8` → `ExportToXML` → `Uitvoeren`
6. Sla het XML-bestand op
7. Importeer het XML-bestand in Exact Online

## 📊 Velden Uitleg

| Veld | Beschrijving | Verplicht | Waarden |
|------|--------------|-----------|---------|
| **Code** | Rekeningnummer | Ja | Tekst (max 20 tekens) |
| **Description** | Omschrijving van de rekening | Ja | Tekst |
| **Type** | Type rekening | Ja | 12, 13, of 20 (zie onder) |
| **BalanceSide** | Debet of Credit | Nee | D (Debet) of C (Credit) |
| **BalanceType** | Balans of W&V | Nee | B (Balans) of W (Winst & Verlies) |
| **IsBlocked** | Geblokkeerd | Nee | 0 (Nee) of 1 (Ja) |
| **SearchCode** | Zoekcode | Nee | Tekst |
| **VATCode** | BTW-code | Nee | Tekst |

## 🔢 Account Type Codes

| Code | Beschrijving |
|------|--------------|
| **12** | Balans: Activa (Assets) |
| **13** | Balans: Passiva (Liabilities) |
| **20** | Winst & Verlies (Profit & Loss) |

## 📝 Voorbeeld Data

De template bevat voorbeelddata:

| Code | Description | Type | BalanceSide | BalanceType |
|------|-------------|------|-------------|-------------|
| 1000 | Kas | 12 | D | B |
| 1100 | Bank | 12 | D | B |
| 1200 | Debiteuren | 12 | D | B |
| 1300 | Crediteuren | 13 | C | B |
| 4000 | Inkopen | 20 | D | W |
| 8000 | Omzet | 20 | C | W |

## 📥 Importeren in Exact Online

1. Log in op Exact Online
2. Ga naar **Financieel** → **Instellingen** → **Grootboekrekeningen**
3. Klik op **Acties** of **Import**
4. Selecteer **XML** als bestandstype
5. Upload het gegenereerde XML-bestand
6. Volg de wizard om de import te voltooien

## ⚙️ Vereisten

- Microsoft Excel 2010 of nieuwer
- Macro-ondersteuning moet ingeschakeld zijn
- Exact Online account met juiste rechten voor import

## 🔧 Macro Uitvoeren

### Optie 1: Macro uitvoeren via sneltoets
1. Druk op `Alt + F8`
2. Selecteer `ExportToXML`
3. Klik op `Uitvoeren`

### Optie 2: Macro bekijken/bewerken
1. Druk op `Alt + F11` om de VBA Editor te openen
2. De macro code staat in Module1
3. Pas aan indien nodig

## 🛠️ Troubleshooting

### Macro's werken niet
- Controleer of macro's zijn ingeschakeld: Bestand → Opties → Vertrouwenscentrum → Instellingen vertrouwenscentrum → Macro-instellingen
- Kies "Alle macro's inschakelen" of "Alle macro's met een melding uitschakelen"

### Import mislukt in Exact Online
- Controleer of alle verplichte velden zijn ingevuld (Code, Description, Type)
- Controleer of de waarden in Type, BalanceSide, BalanceType, IsBlocked correct zijn
- Test eerst met een klein aantal rekeningen

### Speciale tekens in beschrijvingen
- De macro handelt automatisch XML special characters af (&, <, >, ", ')
- Als er problemen zijn, vermijd deze tekens in de beschrijvingen

## 📄 Licentie

Dit is een open template die vrij gebruikt mag worden.

## 🤝 Bijdragen

Verbeteringen en suggesties zijn welkom! Open een issue of pull request.

## 📧 Contact

Voor vragen of ondersteuning, open een issue in deze repository.

---

**Let op:** Deze template is niet officieel onderdeel van Exact Online. Het is een hulpmiddel om het importproces te vergemakkelijken.