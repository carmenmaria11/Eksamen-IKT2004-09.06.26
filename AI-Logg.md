# AI-Logg
### Her vil du se prompts og svar fra AI bruk
### Innhold: 
1. Promt for å hjelpe med time management: Gemini Pro
2. Promt for å hjelpe med kommandoene til å skille enhetene til bedrifter sånn at de ikke kan spionere på hverandre: Gemini Pro

### Prompts og svar:
### Prompt 1: Brukt for time management

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

### Svar:
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

### Prompt 2: Promt for å hjelpe med kommandoene til å skille enhetene til bedrifter sånn at de ikke kan spionere på hverandre

### Prompt:
Jeg har laget et nettverk til små bedrift i Cisco Packet Tracer. Jeg har delt opp i 2 bedrifter som hver har 2 pcer og 1 printer. Venstre side er Bedrift 1 og har IPadreser som starter på 192.168.10.X. Høyre side er Bedrift 2 og starter på 192.168.20.X. Jeg har lagt inn alle IPadressene på pcene selv. nå trenger jeg hjelp til å låse switchen slik at de to sidene blir helt seperert. jeg trenger også kommandoen til ruteren som lager en brannmurregel slik at ingen av enhetene til bedrift a kan snakke med noen fra bedrift B. Kan du gi meg kodene og forklare enkelt hva de gjør sånn at jeg for god oversikt?

### Svar:
Dette er et veldig klassisk og godt oppsett for å lære nettverkssikkerhet! For å oppnå det du ønsker, må vi gjøre to ting:

1. **På switchen:** Opprette to **VLAN** (Virtuelle lokalnettverk). Dette gjør at switchen oppfører seg som om den er to fysisk separate switcher, slik at trafikk ikke kan flyte direkte mellom dem på lag 2.
2. **På ruteren:** Lage en **ACL** (Access Control List), som fungerer som en brannmurregel. Siden ruteren i utgangspunktet vil prøve å rute trafikk mellom de to nettene, bruker vi denne regelen til å stoppe den trafikken.

Her er steg-for-steg-kommandoene du trenger for å låse ned nettverket.

## Konfigurasjon i Packet Tracer

1. **Steg 1: Del opp switchen i VLAN:** Gjøres på switchen.
Klikk på switchen, gå til **CLI**-fanen, trykk Enter og lim inn følgende koder.

*Merk: I eksempelet under antar jeg at Bedrift 1 bruker portene FastEthernet 0/1 til 0/3, og Bedrift 2 bruker portene 0/4 til 0/6. Du må endre portnumrene så de matcher der du har plugget inn kablene dine.*

```text
enable
configure terminal

# Opprett VLAN for Bedrift 1
vlan 10
name Bedrift_1
exit

# Opprett VLAN for Bedrift 2
vlan 20
name Bedrift_2
exit

# Legg portene til Bedrift 1 inn i VLAN 10 (tilpass portene til dine)
interface range fa0/1 - 3
switchport mode access
switchport access vlan 10
exit

# Legg portene til Bedrift 2 inn i VLAN 20 (tilpass portene til dine)
interface range fa0/4 - 6
switchport mode access
switchport access vlan 20
exit

```

**Hva gjør dette?** Vi forteller switchen at portene for Bedrift 1 og Bedrift 2 tilhører helt forskjellige verdener. Enheter i VLAN 10 kan nå overhodet ikke se eller snakke med enheter i VLAN 20 gjennom switchen.


2. **Steg 2: Opprett brannmurreglene (ACL):** Gjøres på ruteren.
Når du bruker en ruter til å binde nettverkene sammen (for eksempel for at begge skal nå internett), vil ruteren automatisk prøve å hjelpe dem med å snakke sammen. For å stoppe dette lager vi en **utvidet ACL** (Extended Access Control List) på ruteren.

Gå inn på ruteren sin **CLI** og skriv:

```text
enable
configure terminal

# Regel for Bedrift 1: Nekt trafikk som skal til Bedrift 2
access-list 101 deny ip 192.168.10.0 0.0.0.255 192.168.20.0 0.0.0.255
access-list 101 permit ip any any

# Regel for Bedrift 2: Nekt trafikk som skal til Bedrift 1
access-list 102 deny ip 192.168.20.0 0.0.0.255 192.168.10.0 0.0.0.255
access-list 102 permit ip any any

```

**Hva gjør dette?**

* `deny ip 192.168.10.0 0.0.0.255 ...`: Forteller ruteren at pakker som kommer fra 10-nettverket og prøver å nå 20-nettverket, skal kastes rett i søpla. `0.0.0.255` er en *wildcard mask* som betyr "gjelder alle adresser i dette subnettet".
* `permit ip any any`: **Veldig viktig!** Cisco-rutere blokkerer *alt* som ikke er spesifikt tillatt som standard. Denne linjen sørger for at alt annet av trafikk (for eksempel ut mot internett) fortsatt er lov.


3. **Steg 3: Aktivér brannmuren på ruterens grensesnitt:** Gjøres på ruteren.
Reglene vi nettopp laget gjør ingenting før vi henger dem på portene (interfacene) der trafikken faktisk går inn i ruteren.

Du må gå inn på interfacene som peker ned mot de to bedriftene (hvis du bruker *Router-on-a-Stick* med subinterfaces, går du inn på f.eks. `.10` og `.20`):

```text
# Gå inn på grensesnittet til Bedrift 1 (bytt ut med ditt interface-navn)
interface gigabitEthernet 0/0.10
ip access-group 101 in
exit

# Gå inn på grensesnittet til Bedrift 2 (bytt ut med ditt interface-navn)
interface gigabitEthernet 0/0.20
ip access-group 102 in
exit

```

**Hva gjør dette?** `ip access-group 101 in` betyr at i det sekundet en pakke beveger seg **inn** i ruteren fra Bedrift 1, sjekker ruteren regelboken vår (Access-list 101). Hvis pakken prøver å besøke Bedrift 2, blir den stoppet i døra.


---

> **Et lite tips når du tester i Packet Tracer:** Bruk det lukkede konvolutt-ikonet (Simple PDU) til å pinge fra en PC i Bedrift 1 til en PC i Bedrift 2. Du vil se at statusen nede i høyre hjørne raskt endrer seg til **Failed**, noe som betyr at den nye brannmuren din gjør akkurat det den skal!
