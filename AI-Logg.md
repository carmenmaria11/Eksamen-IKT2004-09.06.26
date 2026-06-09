# AI-Logg
### Her vil du se prompts og svar fra AI bruk
###Innhold: 
1. Promt for å hjelpe med time management: Gemini Pro

### Prompts og svar:
**Prompt 1: Brukt for time management**

**Prompt:**
Lag en plan for denne eksamen, jeg vil helst gjøre alt selv, altså bruke minst mulig ai eller evt lære fra ai. lag en plan med programmene jeg trenger, ting som er nytting å søke på og hvor mye tid jeg må bruke på hver, jeg må også lage presentasjon. jeg har 4 timer. Eksamensoppgave: Situasjonsbeskrivelse: Kontorutleie
Et selskap som driver med kontorutleie, trenger å sette opp sitt nettverk og webbasert løsning for bedriften. Slik at de kan tilby sine kontortjenester til sine private kunder og små bedrifter.
Hver bedrift har 1-10 ansatte og  disse skal ha it utstyr som kan kommunisere med hverandre (for eksempel skal deres PC kunne koble seg til deres nettverksprinter)
En bedrift skal ikke kunne nå andre bedrifts it utstyr (subnet).
Oppgave 1 utvikling 
- webløsning med beskrivelse av tjenestene (for potensielle nye kunder= 
- web løsning med tilgang til dokumentasjon av nettverksoppsett, for eksisterende kunder (for eksempel DNS-oppsett og lignende)
Oppgave 2 drift:
Alt utstyr er ikke kommet i tide, men teknikeren trenger å vite hvordan nettverket skal se ut. lag en skisse på:
- oppsett av nettverket
- eventuell subnettverk
-brannmur/portstyring
Oppgave 3 Brukerstøtte
lag følgebe veukeder for Active Directory:
 husk opprette bruker
-hvordan sette opp tilgang på mappe og filnivå
husk at veilederen skal være brukervennlig.

**Svar:**
Dette er en omfattende oppgave for fire timer, spesielt når du vil gjøre mest mulig selv. For å komme i mål må du være streng med tidsbruken og fokusere på funksjonalitet fremfor perfeksjon.

## 🕒 Tidsplan (Total tid: 4 timer)

| Tid | Aktivitet | Fokusområde |
| --- | --- | --- |
| **00:00 - 00:45** | **Oppgave 2: Drift & Nettverk** | Designe subnett og brannmur-logikk. |
| **00:45 - 02:00** | **Oppgave 1: Utvikling** | Kode den grunnleggende webløsningen (HTML/CSS). |
| **02:00 - 02:45** | **Oppgave 3: Brukerstøtte** | Skrive veiledninger (skjermbilder og tekst). |
| **02:45 - 03:30** | **Presentasjon** | Samle alt i en rød tråd. |
| **03:30 - 04:00** | **Buffer & Kvalitetssjekk** | Sjekke skrivefeil, linker og lagre alt. |

---

## 🛠️ Verktøy du bør bruke

* **Nettverksskisse:** [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer) (hvis du har det), eller [Lucidchart](https://www.lucidchart.com) / [Draw.io](https://app.diagrams.net) for selve skissen.
* **Utvikling:** [Visual Studio Code](https://code.visualstudio.com/) (VS Code).
* **Presentasjon:** PowerPoint eller Canva.
* **Dokumentasjon:** Word eller Google Docs (for veiledninger før de limes inn i presentasjonen).

---

## 🌐 Trinn 1: Drift & Nettverk (45 min)

Målet her er å isolere bedriftene fra hverandre.

* **Logikk:** Bruk **VLAN** (Virtual Local Area Network) for å skille bedriftene. Hver bedrift får sitt eget subnett (f.eks. Bedrift A: `192.168.10.0/24`, Bedrift B: `192.168.20.0/24`).
* **Brannmur:** Konfigurer ACL (Access Control Lists) som tillater trafikk internt i subnettet, men blokkerer trafikk mellom subnettene.
* **Søk etter:** *"How to design small business network with VLAN isolation"*, *"VLAN subnetting table 10 hosts"*, *"Basic firewall rules for inter-VLAN routing"*.

---

## 💻 Trinn 2: Utvikling (75 min)

Hold det enkelt. Lag én hovedside (index.html) og én side for eksisterende kunder (info.html).

* **Hva du må kode:**
* En enkel navigasjonsmeny (Nav bar).
* Seksjoner som beskriver kontortjenestene (møterom, kaffe, wifi).
* En tabell eller liste på info-siden som viser DNS-innstillinger (f.eks. `Primær DNS: 8.8.8.8`).


* **Læringstips:** Bruk AI til å forklare *hvorfor* en kodebit fungerer, heller enn å be den skrive alt. Spør f.eks.: *"Hvordan lager jeg en enkel navigasjonsmeny i CSS som holder seg på toppen?"*
* **Søk etter:** *"Simple HTML/CSS landing page tutorial"*, *"HTML table for documentation"*, *"Responsive CSS navigation bar"*.

---

## 👤 Trinn 3: Brukerstøtte (45 min)

Her skal du være pedagogisk. Tenk at en som ikke kan IT skal forstå dette.

* **Active Directory:** Lag punktlister.
* *Opprette bruker:* Start -> AD Users and Computers -> Høyreklikk -> New User.
* *Tilgang:* Høyreklikk mappe -> Properties -> Security -> Edit -> Add (velg bruker/gruppe).


* **Søk etter:** *"Step by step guide create user Active Directory"*, *"NTFS permissions vs Share permissions guide"*.

---

## 📊 Trinn 4: Presentasjon (45 min)

Dette er "salget" av løsningen din.

1. **Intro:** Hva er behovet til kontorutleieren?
2. **Nettverket:** Vis skissen din og forklar hvorfor VLAN er trygt.
3. **Nettsiden:** Vis frem koden eller åpne siden i en nettleser.
4. **Drift:** Vis AD-veilederne dine.
5. **Konklusjon:** Hvordan løser dette kundens problem?

---

> **Tips til eksamen:**
> Ikke bruk for lang tid på å finne den "perfekte" fargen på nettsiden. Sensor ser etter teknisk forståelse og evne til å forklare *hvorfor* du har valgt subnettmaskene og brannmurreglene du har satt opp.
