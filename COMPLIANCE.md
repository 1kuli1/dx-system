# DX Centralen – efterlevnadschecklista

Senast genomgången: 2026-10-06

Detta är en praktisk arbetslista, inte juridisk rådgivning. Målet är att DX Centralen, DX Start, Receiver Hub, Asta och DX Academy ska byggas enligt relevanta EU-regler och svensk genomförandelagstiftning.

## 1. Digital tillgänglighet

Mål: minst WCAG 2.1 nivå AA / relevanta delar av EN 301 549, samt där det är praktiskt även förbättringar från WCAG 2.2.

Status:
- [x] `lang="sv"` på huvudsidor.
- [x] Responsiv viewport.
- [x] Skip-länkar till huvudinnehåll.
- [x] Semantiska `nav`- och `main`-landmärken på huvudsidor.
- [x] Synlig tangentbordsfokus.
- [x] Knappar har explicit `type="button"`.
- [x] Externa länkar som öppnas i ny flik har `noopener/noreferrer`.
- [x] Receiver Hubs sökfält har programmatisk etikett.
- [x] Receiver Hubs upprepade Öppna/Favorit-knappar har kontextuella tillgängliga namn.
- [x] Dynamiska statusmeddelanden på Asta/DX Start har live-regioner där relevant.
- [x] Kända låga kontraster i Receiver Hub/Academy rättade.
- [ ] Manuell test med endast tangentbord.
- [ ] Manuell test med skärmläsare.
- [ ] Test vid 200 % och 400 % zoom/reflow.
- [ ] Test i mobil, surfplatta och desktop efter varje större ändring.
- [ ] Kontroll av formulärfel och felmeddelanden mot WCAG 3.3.x.
- [ ] Kontroll av tabellernas läsordning och mobilpresentation.
- [ ] Publicera tillgänglighetsinformation/redogörelse när ansvarig aktör och kontaktväg är fastställda.

## 2. Tillgänglighetslagen / European Accessibility Act

Svensk lag: lag (2023:254) om vissa produkters och tjänsters tillgänglighet (LPTT), som genomför direktiv (EU) 2019/882.

Att bedöma:
- [ ] Om verksamheten är ett mikroföretag (färre än 10 anställda och högst 2 miljoner euro i årsomsättning/balansomslutning). Mikroföretag är undantagna från tjänstekraven i LPTT.
- [ ] Om och vilka delar av DX Academy utgör e-handelstjänst, dvs. används för att ingå konsumentavtal på distans.
- [ ] Om en e-handelstjänst lanseras: dokumentera hur tjänsten uppfyller tillgänglighetskraven och publicera tillgänglighetsinformation.

## 3. GDPR och personuppgifter

DX-loggar kan innehålla personuppgifter, exempelvis namn, kontaktuppgifter eller radioamatörers anropssignaler.

Att göra:
- [ ] Fastställ personuppgiftsansvarig och kontaktuppgifter.
- [ ] Kartlägg vilka personuppgifter som lagras lokalt respektive skickas till Google Drive.
- [ ] Fastställ ändamål, rättslig grund och lagringstid.
- [ ] Skapa integritetsinformation enligt GDPR artikel 13.
- [ ] Beskriv mottagare/personuppgiftsbiträden och eventuella tredjelandsöverföringar.
- [ ] Beskriv registrerades rättigheter och kontaktväg.
- [ ] Bedöm om personuppgiftsbiträdesavtal krävs för Google-tjänster.

Särskild risk:
- [ ] Nuvarande Drive-synk använder en fast Google Apps Script-endpoint i klientkoden utan synlig användarautentisering eller per-användaridentifiering. Detta måste säkerhetsgranskas innan systemet används som publik fleranvändartjänst.

## 4. Kakor, localStorage och terminalinformation

- [x] Systemet använder localStorage för kärnfunktioner som loggar och inställningar.
- [ ] Dokumentera vilka nycklar som lagras och varför.
- [ ] Bedöm vilka lagringar som är strikt nödvändiga för uttryckligen begärda funktioner.
- [ ] Om analys, marknadsföring eller annan icke-nödvändig lagring införs: inhämta förhandssamtycke och gör det lika lätt att neka/återkalla.
- [ ] Publicera lättillgänglig information om lokal lagring/kakor.

## 5. Asta och AI-förordningen

- [x] Asta anges tydligt vara en AI-assistent.
- [x] Det framgår att ChatGPT från OpenAI öppnas och att användaren då interagerar med ett AI-system.
- [x] Asta skickar inte automatiskt frågan till ChatGPT; användaren väljer själv att öppna tjänsten.
- [ ] Integritetsinformationen ska förklara att eventuell text, bild eller ljud som användaren själv lämnar i ChatGPT hanteras av den externa tjänsten enligt dess villkor.

## 6. DX Academy, e-handel och konsumenträtt

Om kurser ska säljas till konsumenter:
- [ ] Företagets/aktörens namn.
- [ ] Geografisk adress.
- [ ] E-post/kontaktuppgifter.
- [ ] Organisationsnummer om sådant finns.
- [ ] Tydligt totalpris och korrekt uppgift om skatter/moms.
- [ ] Betalnings-, leverans- och avtalsvillkor.
- [ ] Information om reklamationsrätt.
- [ ] Information om 14 dagars ångerrätt där den gäller.
- [ ] Ångerblankett.
- [ ] Om avtal sluts på webbplats/app: en tydlig ångerfunktion enligt reglerna som gäller sedan 19 juni 2026.
- [ ] Om betalningsknapp införs: tydlig information om betalningsskyldighet.
- [ ] Bekräftelse av avtalet i varaktig form.
- [ ] Tillgänglig betalnings-, identifierings- och säkerhetsprocess om e-handeln omfattas av LPTT.

## 7. Externa tjänster, länkar och innehåll

- [x] Onödig Leaflet-CDN-laddning borttagen från DX Start.
- [ ] Inventera alla externa SDR-, katalog-, Google- och AI-länkar.
- [ ] Informera tydligt om att externa tjänster har egna villkor och integritetspolicyer.
- [ ] Undvik att kopiera upphovsrättsskyddade bilder, logotyper, databaser eller längre texter utan tillstånd.
- [ ] Kontrollera rättigheter/licenser för eventuella kartbilder, ljudfiler och kursmaterial.

## 8. Regler som i nuläget sannolikt inte träffar kärntjänsten

Dessa ska omprövas om funktionerna ändras:
- Digital Services Act: blir mer relevant om tjänsten börjar lagra/förmedla användargenererat innehåll åt allmänheten.
- NIS2/cybersäkerhetsregler: beror på verksamhetens sektor, storlek och roll.
- Betaltjänstregler: blir relevanta om betalning hanteras på annat sätt än genom en extern betaltjänstleverantör.

## Nästa beslut som behövs

1. Fastställ den juridiska aktör som står bakom DX Academy/DX Centralen och vilken kontaktadress/e-post som ska publiceras.
2. Bestäm om kurser ska kunna köpas/avtalas direkt online eller endast marknadsföras.
3. Säkerhetsgranska och separera Google Drive-synken innan publik fleranvändaranvändning.


## 9. Katastrof-DX / nödradiolyssning

- [x] Katastrof-DX är uttryckligen ett lyssnar- och dokumentationsverktyg och startar ingen sändning.
- [x] Tydlig instruktion att aldrig störa nödradio eller aktiv EmComm-trafik.
- [x] Skillnad mellan bekräftat nödradionät, bevakningsläge och ingen känd aktivering.
- [x] Frekvenslistor presenteras som startpunkter och ska verifieras mot aktuella officiella källor.
- [x] Separat Katastrof-DX-loggbok så att krisobservationer inte blandas ihop med ordinarie DX-logg.
- [x] Katastrofloggen lagras lokalt på enheten och kan exporteras av användaren.
- [x] Varning mot att lagra eller sprida onödiga känsliga personuppgifter om drabbade personer.
- [ ] Bedöm ytterligare rättsliga krav innan automatisk vidarepublicering, delning eller central insamling av katastrofloggar införs.
- [ ] Om automatisk hämtning av händelser/frekvenser införs: dokumentera källa, uppdateringstid och datalicens samt undvik att visa obekräftad information som officiell.
