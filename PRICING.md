# Preisübersicht für Usenet-Streaming-Projekte 2026

Die Gesamtkosten für ein vollständiges Usenet-Streaming-Setup liegen zwischen **€5 und €50 pro Monat**, abhängig von der gewählten Konfiguration. Während zentrale Komponenten wie Stremio, Caddy und DuckDNS vollständig kostenlos sind, entstehen die Hauptkosten durch Usenet-Provider und VPS-Hosting. Die aktuellen Black-Friday-Deals bei Usenet-Providern bieten außergewöhnliche Einsparungen von bis zu **92%** – wer jetzt zuschlägt, sichert sich Preise von unter **€2 pro Monat**.

---

## Medien-Datenbanken: APIs für Metadaten und Poster

Die vier wichtigsten Medien-APIs unterscheiden sich stark in ihrem Preismodell. **TMDB** bleibt für nicht-kommerzielle Projekte vollständig kostenlos – das Unternehmen hat in über 10 Jahren Betrieb noch nie Gebühren erhoben. Lediglich die Attribution (Logo + Hinweis) ist erforderlich. Für kommerzielle Nutzung werden Lizenzen individuell verhandelt.

**TVDB** hingegen staffelt seit 2020 nach Unternehmensumsatz: Projekte unter $50.000 Jahresumsatz nutzen die API kostenlos. Darüber beginnen Lizenzen bei **€850/Jahr** (bis $250.000 Umsatz) und steigen auf **€8.500/Jahr** für größere Unternehmen. Alternativ bietet TVDB ein User-Subscription-Modell für **€10,19/Jahr** pro Endnutzer.

| Dienst | Kostenlos | Einstiegspreis Premium |
|--------|-----------|------------------------|
| **TMDB** | ✅ Ja (Attribution nötig) | Individuell verhandelbar |
| **TVDB** | ✅ Ja (unter $50k Umsatz) | €10,19/Jahr (User-Abo) |
| **RPDB** | ❌ Nein | **€1,85/Monat** (Tier 1) |
| **MDBList** | ✅ Ja (1.000 API-Calls/Tag) | **€1,20/Monat** |

**RPDB** bietet keine kostenlose Option – alle Poster-Features erfordern ein Patreon-Abo. Die Tiers reichen von €1,85/Monat (50.000 Requests) bis €28/Monat (750.000 Requests). Interessant: Lifetime-Optionen für **€96 (Tier 2)** oder **€168 (Tier 3)** amortisieren sich nach etwa 2 Jahren.

**MDBList** überzeugt mit einem großzügigen Free-Tier und günstigen Premium-Optionen direkt in EUR. Der Basic-Plan für €1,20/Monat (oder **€10/Jahr** mit 30% Rabatt) deckt die Bedürfnisse der meisten Projekte ab.

---

## Usenet-Provider: Spektakuläre Bundle-Deals aktiv

Die drei führenden Provider – Newshosting, Easynews und Eweka – gehören zur selben Unternehmensgruppe, bieten aber unterschiedliche Backbones und Features. Aktuell sind noch **Black-Friday-Deals verfügbar**, die das beste Preis-Leistungs-Verhältnis des Jahres bieten.

### Newshosting Mega-Bundle (Top-Empfehlung)

Das spektakulärste Angebot ist das **Newshosting Bundle für €23 (15 Monate)** – das entspricht nur **€1,54/Monat**:

- Newshosting Unlimited (100 Connections)
- Easynews Unlimited (Web-Streaming)
- Tweaknews Unlimited (EU-Backbone)
- PrivadoVPN inklusive
- 6.348+ Tage Retention

Nach Ablauf: €66/Jahr (€5,99/Monat). Der Deal ist **stapelbar** – mehrere Käufe verlängern die Laufzeit.

### Eweka für EU-Nutzer

Eweka mit eigenem Tier-1-Backbone in Amsterdam bietet **€37,50 für 15 Monate (€2,50/Monat)**:

- Eweka Unlimited + Easynews inklusive
- PrivadoVPN inklusive
- 50 Connections, 6.349+ Tage Retention
- Direkte EUR-Abrechnung, DSGVO-konform

| Provider | Deal-Preis | Regulär (jährlich) | Besonderheit |
|----------|------------|--------------------|--------------|
| **Newshosting Bundle** | €1,54/Mo | €5,99/Mo | 3 Provider + VPN |
| **Eweka Bundle** | €2,50/Mo | €5,99/Mo | EU-Backbone |
| **Easynews Annual** | - | €5,51/Mo | Browser-Streaming |

---

## VPS-Hosting: Deutsche Anbieter im Vergleich

Für Usenet-Streaming sind **hoher Traffic** und **ausreichend RAM** entscheidend. Vier deutsche Anbieter dominieren den Markt:

### IONOS VPS

| Tarif | Preis/Monat | vCPU | RAM | NVMe | Traffic |
|-------|-------------|------|-----|------|---------|
| **VPS S** | **€2** | 1 | 1 GB | 10 GB | Unbegrenzt |
| **VPS M** | €4 | 2 | 2 GB | 80 GB | Unbegrenzt |
| **VPS L** | €6 | 4 | 4 GB | 160 GB | Unbegrenzt |

IONOS punktet mit **unbegrenztem Traffic** und deutschen Rechenzentren. Für einfache Setups reicht bereits der VPS S für €2/Monat.

### Hetzner Cloud (Preis-Leistungs-Sieger)

| Tarif | Preis/Monat | vCPU | RAM | NVMe | Traffic |
|-------|-------------|------|-----|------|---------|
| **CX23** | **€3,49** | 2 | 4 GB | 40 GB | 20 TB |
| **CX33** | €5,49 | 4 | 8 GB | 80 GB | 20 TB |
| **CAX11** (ARM) | €3,79 | 2 | 4 GB | 40 GB | 20 TB |

Hetzner bietet das **beste Gesamtpaket**: 20 TB inkludierter Traffic, NVMe-Storage, stundenbasierte Abrechnung und exzellente Netzwerkanbindung in Nürnberg und Falkenstein.

### Weitere Alternativen

- **Netcup VPS 250 G11s**: €3,99/Mo (2 vCore, 2 GB RAM, 64 GB SSD)
- **Contabo Cloud VPS 10**: €5,36/Mo (6 vCPU, **12 GB RAM**, 32 TB Traffic) – bestes RAM/Preis-Verhältnis

**Empfehlung für Usenet-Streaming**: **Hetzner CX33 für €5,49/Monat** – ausgewogenes Verhältnis aus Leistung, Traffic und Zuverlässigkeit.

---

## Kostenlose Dienste: DuckDNS, Stremio und Caddy

Drei zentrale Komponenten des Stacks kosten **nichts**:

**DuckDNS** bleibt vollständig kostenlos – bis zu 5 Subdomains pro Account, IPv4/IPv6, Wildcard-Support und SSL. Es gibt kein Premium-Modell, nur freiwillige Spenden. Alternativen wie Dynu oder No-IP bieten ähnliche kostenlose Tiers.

**Stremio** ist ebenfalls 100% kostenlos und Open Source. Es gibt keine offiziellen Premium-Features. Optionale Kosten entstehen nur durch Drittanbieter-Dienste wie Real-Debrid (€3-5/Monat) oder Premiumize (€10/Monat) für beschleunigte Streams.

**Caddy** als Reverse Proxy ist unter Apache 2.0 Lizenz vollständig kostenlos – alle Features inklusive automatischer HTTPS-Zertifikate via Let's Encrypt. Die kostenpflichtigen Sponsorship-Tiers (ab $25/Monat) sind reine Support-Pakete ohne zusätzliche Funktionen.

---

## NZB-Indexer: SceneNZBs und Alternativen

**SceneNZBs** ist spezialisiert auf deutschen Content und bietet offene Registrierung mit einem kostenlosen Tier (5-10 NZB-Downloads/Tag). VIP-Preise sind nicht öffentlich dokumentiert.

Empfehlenswerte Alternativen in EUR:

| Indexer | Kostenlos | Premium | Besonderheit |
|---------|-----------|---------|--------------|
| **DrunkenSlug** | ✅ 5 NZB/Tag | **€10-20/Jahr** | Invite-only, hohe Qualität |
| **NZBgeek** | ✅ Trial | **€11/Jahr**, €74 Lifetime | Offene Registrierung |
| **NZBFinder** | ✅ Limitiert | €10-35/Jahr | Gute Automation-Integration |

---

## Gesamtkostenrechnung: Drei Szenarien

### Minimal-Setup (€8-10/Monat)
- IONOS VPS S: €2
- Eweka Bundle (umgerechnet): €2,50
- TMDB + MDBList Free: €0
- DuckDNS + Stremio + Caddy: €0
- **Gesamt: ~€4,50/Monat**

### Standard-Setup (€15-20/Monat)
- Hetzner CX33: €5,49
- Newshosting Bundle: €1,54 (Deal) oder €5,99
- MDBList Basic: €1,20
- RPDB Tier 2: €3,70
- NZB-Indexer (DrunkenSlug): €0,83/Monat
- **Gesamt: ~€13-17/Monat**

### Premium-Setup (€25-35/Monat)
- Hetzner CCX13 (dediziert): €12,49
- Newshosting Bundle + Eweka Backup: €8
- MDBList VIP: €5
- RPDB Tier 3: €6,50
- Mehrere NZB-Indexer: €2-3
- **Gesamt: ~€34/Monat**

---

## Fazit und Handlungsempfehlungen

Die **Black-Friday-Deals bei Usenet-Providern** sollten priorisiert werden – sie laufen bald aus und bieten Ersparnisse von über €100 jährlich. Das Newshosting-Bundle für €23/15 Monate ist das beste Angebot am Markt.

Für den VPS empfiehlt sich **Hetzner** aufgrund des inkludierten 20-TB-Traffics und der deutschen Rechenzentren. Bei den Medien-APIs reichen für Hobby-Projekte die kostenlosen Tiers von TMDB und MDBList aus – RPDB ist nur notwendig, wenn Rating-Overlays auf Postern gewünscht sind.

Die Infrastruktur-Komponenten DuckDNS, Stremio und Caddy kosten nichts und erfordern keine Kompromisse bei der Funktionalität. Ein vollständiges, professionelles Setup ist damit bereits ab **€10-15 pro Monat** realisierbar.