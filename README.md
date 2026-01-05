# 🎬 Usenet Streamer - Komplette Dokumentation & Setup-Anleitung

Eine umfassende deutschsprachige Dokumentation für das Einrichten eines privaten **Usenet-Streaming-Setups** mit Stremio, NZBDav und allen benötigten Services.

## 📋 Inhaltsverzeichnis

- [Was ist Usenet Streamer?](#was-ist-usenet-streamer)
- [Dokumentation](#dokumentation)
- [Systemanforderungen](#systemanforderungen)
- [Kosten-Übersicht](#kosten-übersicht)
- [Schnelleinstieg](#schnelleinstieg)
- [Tipps für Anfänger](#tipps-für-anfänger)
- [Häufig gestellte Fragen](#häufig-gestellte-fragen)
- [Lizenz](#lizenz)

---

## Was ist Usenet Streamer?

**Usenet Streamer** ist ein Stremio Addon, das es dir ermöglicht, NZB-Dateien aus dem Usenet direkt über Stremio zu streamen. 

Das Setup besteht aus mehreren Komponenten:

- **Stremio**: Media-Center zum Verwalten und Streamen deiner Inhalte
- **Usenet Streamer Addon**: Integration in Stremio für Usenet-Streaming
- **NZBDav**: WebDAV-Interface zur Verwaltung von Usenet-Inhalten
- **Usenet-Provider** (Newshosting, Easynews, Eweka): Zugang zum Usenet-Netzwerk
- **NZB-Indexer** (SceneNZBs, DrunkenSlug): Kataloge zum Finden von Inhalten
- **Metadata-Services** (TMDB, TVDB, RPDB): Zusätzliche Informationen und Poster
- **VPS/Server**: Hosting für das Setup

Diese Dokumentation führt dich durch die **komplette Installation und Konfiguration** aller Komponenten.

---

## 📚 Dokumentation

Dieses Repository enthält folgende Dokumentationen:

### Hauptanleitungen

- **[Einsteiger-Guide](docs/beginners-guide.md)** ⭐ 
  - Schritt-für-Schritt Installationsanleitung
  - VPS Mieten und Einrichten
  - Docker Installation
  - Docker Compose Setup
  - Firewall-Konfiguration
  - Caddy HTTPS-Setup
  - Komplette Checkliste

- **[Addons-Konfiguration](docs/addons.md)** 
  - AIOStreams Addon Setup
  - AIOCatalogs Integration
  - AIOMetadata Konfiguration
  - TMDB und TVDB Integration
  - RPDB für hochwertige Poster
  - MDBList für personalisierte Listen

- **[TMDB API Setup](docs/tmdb-api.md)** 
  - TheMovieDB API-Schlüssel generieren
  - Konfiguration in Stremio Addons
  - Kostenlose Nutzung erklärt

### Zusätzliche Ressourcen

- **[Preisübersicht (PRICING.md)](PRICING.md)** 💰
  - Alle Services und deren Kosten
  - Usenet-Provider Vergleich
  - VPS-Hosting Optionen
  - Aktuelle Black-Friday-Deals
  - 3 komplette Kostenszenarien

---

## 🖥️ Systemanforderungen

### Hardware

| Anforderung | Mindestens | Empfohlen |
|------------|-----------|-----------|
| **CPU** | 1 vCore | 2+ vCores |
| **RAM** | 1 GB | 4+ GB |
| **Festplatte** | 20 GB | 50+ GB |
| **Netzwerk** | Unbegrenzt | 5 Mbps+ |

### Software

- **Linux** (Ubuntu 22.04 LTS oder neuer empfohlen)
- **Docker** und **Docker Compose**
- **SSH-Zugriff** auf einen Server/VPS
- **Bash** Shell

### Externe Accounts

✅ = Kostenlos | 💰 = Kostenpflichtig | ⚡ = Optional

| Service | Notwendig | Kosten | Anmerkung |
|---------|-----------|--------|----------|
| **Stremio** | ✅ | ✅ Kostenlos | Media Center |
| **Usenet-Provider** | ✅ | 💰 €1,50-€6/Mo | Newshosting, Easynews, Eweka |
| **NZB-Indexer** | ✅ | ✅ Kostenlos-💰 | SceneNZBs, DrunkenSlug, NZBgeek |
| **VPS/Server** | ✅ | 💰 €2-€15/Mo | IONOS, Hetzner, Netcup |
| **TMDB API** | ⚡ | ✅ Kostenlos | Metadaten und Poster |
| **TVDB API** | ⚡ | ✅ Kostenlos | TV-Serie Details |
| **RPDB** | ⚡ | ✅ Kostenlos-💰 | Hochwertige Poster mit Ratings |
| **MDBList** | ⚡ | ✅ Kostenlos-💰 | Personalisierte Listen |
| **DuckDNS** | ⚡ | ✅ Kostenlos | Remote-Zugriff (HTTPS) |
| **PrivadoVPN** | ⚡ | ✅ Gratis (im Bundle) | Datenschutz (optional) |

---

## 💰 Kosten-Übersicht

Die monatlichen Gesamtkosten hängen stark ab von der gewählten Konfiguration und den genutzten Services.

### Kostenübersicht nach Szenario

| Szenario | VPS | Usenet | APIs | Indexer | **Gesamt/Monat** |
|----------|-----|--------|------|---------|-----------------|
| **Budget** | €2 | €2,50 | €0 | €0 | **~€4,50** |
| **Standard** | €5,49 | €1,54* | €5 | €1 | **~€13** |
| **Premium** | €12,49 | €8 | €12 | €3 | **~€35** |

*Newshosting Bundle Deal (limitiert verfügbar)

### Aktuelle Black-Friday-Deals

⚡ **ZEITLICH BEGRENZT** - Diese Angebote sollten priorisiert werden:

- **Newshosting Bundle**: €23 für 15 Monate (€1,54/Mo) - 3 Provider + VPN
- **Eweka Bundle**: €37,50 für 15 Monate (€2,50/Mo) - EU-Backbone
- **Newshosting Annual**: €72/Jahr (€6/Mo) regulär

→ **Detaillierte Kostenanalyse**: Siehe [PRICING.md](PRICING.md)

---

## 🚀 Schnelleinstieg

### 1️⃣ Server/VPS wählen und mieten

Beliebte deutsche VPS-Anbieter:

```bash
# IONOS VPS-S (€2/Monat)
https://www.ionos.de/server/vps

# Hetzner Cloud CX33 (€5,49/Monat)
https://www.hetzner.com/cloud

# Netcup VPS 250 G11s (€3,99/Monat)
https://www.netcup.com/de/server/vps
```

Wähle Ubuntu 22.04 LTS oder neuer als Betriebssystem.

### 2️⃣ SSH-Verbindung aufbauen

```bash
ssh root@deine-vps-ip
# Gib das Passwort ein (von deinem Provider)
```

### 3️⃣ Firewall konfigurieren

Öffne folgende Ports:
- **80** (HTTP, für Let's Encrypt)
- **443** (HTTPS)
- **7000** (Usenet Streamer)
- **3000** (NZBDav - optional, nur lokal)
- **22** (SSH)

### 4️⃣ Docker installieren

```bash
sudo apt update
sudo apt install -y docker.io docker-compose-plugin
```

### 5️⃣ Setup klonen und starten

```bash
mkdir -p ~/usenetstack && cd ~/usenetstack
docker-compose pull
docker-compose up -d
```

### 6️⃣ Webinterfaces öffnen

- **NZBDav**: `http://deine-vps-ip:3000`
- **Usenet Streamer Admin**: `http://deine-vps-ip:7000/<ADDON_SECRET>/admin/`

### 7️⃣ In Stremio hinzufügen

Manifest-URL in Stremio eingeben:
```
https://deine-vps-ip:7000/<ADDON_SECRET>/manifest.json
```

👉 **Detaillierte Schritte**: [Einsteiger-Guide](docs/beginners-guide.md)

---

## 💡 Tipps für Anfänger

### 1. Welchen Usenet-Provider soll ich wählen?

**Für Anfänger**: Newshosting Bundle (€1,54/Mo) - alles inklusive
**Für Deutsch-Content**: Eweka (EU-Backbone, DSGVO-konform)
**Für Englisch-Content**: Easynews (Web-Streaming Integration)

→ Siehe [PRICING.md](PRICING.md) für detaillierten Vergleich

### 2. Welchen NZB-Indexer soll ich wählen?

**Kostenlos, Anfänger**: SceneNZBs (Deutsch) oder NZBgeek (Englisch)
**Bessere Qualität**: DrunkenSlug (€10-20/Jahr, Invite-only)
**Mit Automation**: DrunkenSlug + NZBFinder

### 3. Lokales Netzwerk oder Remote?

**Lokal (Heimnetzwerk)**:
- Einfacher (keine DuckDNS nötig)
- Zugriff nur zuhause möglich
- URL: `http://192.168.1.x:7000`

**Remote (von überall)**:
- DuckDNS-Account kostenlos erstellen
- Caddy Reverse Proxy einrichten
- HTTPS automatisch via Let's Encrypt
- URL: `https://dein-name.duckdns.org`

→ Siehe [Einsteiger-Guide - DuckDNS & Caddy](docs/beginners-guide.md#4-configure-duckdns)

### 4. Welche Addons sollte ich nutzen?

**Mindestens**:
- Usenet Streamer (dieses Setup)
- AIOStreams oder AIOCatalogs (für Kataloge)

**Zusätzlich empfohlen**:
- AIOMetadata (für bessere Poster und Metadaten)
- Real-Debrid oder Premiumize (für zusätzliche Quellen)

→ Siehe [Addons-Konfiguration](docs/addons.md)

### 5. Ist mein Setup sicher?

**Ja**, mit folgenden Massnahmen:
- ✅ HTTPS (via Caddy & Let's Encrypt)
- ✅ Geheimes Token (ADDON_SHARED_SECRET)
- ✅ Firewall-Ports begrenzen
- ✅ Regelmäßige Backups
- ⚡ Optional: VPN für Usenet-Traffic

### 6. Wie oft sollte ich aktualisieren?

**Regelmäßig** (z.B. monatlich):
```bash
cd ~/usenetstack
docker-compose pull
docker-compose up -d
```

---

## ❓ Häufig gestellte Fragen

### F: Ist das Setup legal?
**A**: Ja, solange du das Usenet-Netzwerk verantwortungsvoll nutzt und lokale Gesetze beachtest. Der Zugriff auf urheberrechtlich geschützte Inhalte ist je nach Region unterschiedlich reguliert.

### F: Kann ich das Setup zwischen mehreren Personen teilen?
**A**: Technisch ja, aber beachte die Nutzungsbedingungen deiner Usenet-Provider und lokale Gesetze. Das Setup ist für persönliche Nutzung ausgelegt.

### F: Brauche ich ein VPN?
**A**: Nicht zwingend erforderlich, aber empfohlen für mehr Privatsphäre. Viele Usenet-Provider bieten VPN-Bundles (z.B. PrivadoVPN mit Newshosting).

### F: Warum ist der Newshosting Deal so günstig?
**A**: Es ist ein **zeitlich limitiertes Black-Friday-Angebot**. Danach kostet es regulär €5,99-€6,99/Monat. Der Deal ist aber **stapelbar** - du kannst mehrmals kaufen für längere Laufzeit.

### F: Was ist der Unterschied zwischen den Usenet-Providern?
**A**: 
- **Newshosting**: Zuverlässig, viele Tage Retention, günstige Bundles
- **Easynews**: Web-Streaming möglich, auch ohne Download
- **Eweka**: EU-Backbone in Amsterdam, DSGVO-konform für Deutsche

### F: Kann ich mehrere Usenet-Provider gleichzeitig nutzen?
**A**: Ja! Definiere mehrere Provider in NZBDav für Failover und Redundanz.

### F: Wie viel Festplatte brauche ich?
**A**: 
- Minimal: 20 GB (nur Docker & Config)
- Mit Pufferung: 50-100 GB empfohlen
- Mit lokalem Cache: Je nach Bedarf

### F: Funktioniert das auch auf einem alten PC zuhause?
**A**: Ja, wenn er läuft und Ubuntu installiert ist. Aber ein VPS ist empfohlen wegen: Zuverlässigkeit, Always-On, statische IP, besseres Netzwerk.

### F: Kann ich NZBDav und Usenet Streamer trennen?
**A**: Das Setup ist eng miteinander verflochten. NZBDav ist notwendig für die WebDAV-Integration. Sie sollten zusammenlaufen.

### F: Wo speichert das System die heruntergeladenen Dateien?
**A**: Die Dateien werden nicht dauerhaft gespeichert, sondern live gestreamt. NZBDav cached möglicherweise Dateitypen, aber der primäre Zweck ist Live-Streaming.

### F: Wie lange Retention brauche ich?
**A**: 
- **Englischer Content**: 3.000+ Tage reichen meist
- **Deutscher Content**: Je neuer, desto besser
- **TV-Serien**: Je mehr Tage, desto mehr Episoden verfügbar

---

## 📖 Weitere Ressourcen

### Offizielle Dokumentation
- [Stremio Dokumentation](https://stremio.github.io/stremio-addons-sdk/docs/)
- [Docker Dokumentation](https://docs.docker.com/)
- [NZBDav GitHub](https://github.com/nzbdav/nzbdav)

### Nützliche Tools
- [OpenSSL Token Generator](https://openssl.tplant.com.au/)
- [Markdown Editor](https://markdowntutorial.com/)
- [DuckDNS](https://www.duckdns.org)
- [Caddy Web Server](https://caddyserver.com)

### Community
- [Stremio Community](https://www.reddit.com/r/Stremio/)
- [Usenet Community](https://www.reddit.com/r/Usenet/)
- [NZB Community](https://www.reddit.com/r/nzbss/)

---

## 🔗 Direkte Links zu Anbietern

### Usenet-Provider
- [Newshosting](https://www.newshosting.com) - Mit Black-Friday Bundle
- [Easynews](https://www.easynews.com) - Web-Streaming
- [Eweka](https://www.eweka.nl) - EU-Friendly
- [Tweaknews](https://www.tweaknews.eu) - Deutsche Alternative

### NZB-Indexer
- [SceneNZBs](https://scenenzbs.com) - Deutsch
- [DrunkenSlug](https://www.drunkenslug.com) - Invite-only
- [NZBgeek](https://www.nzbgeek.info) - Offene Registrierung
- [NZBFinder](https://www.nzbfinder.com) - API-Zugang

### VPS-Anbieter (Deutsch)
- [IONOS VPS](https://www.ionos.de/server/vps) - €2/Mo
- [Hetzner Cloud](https://www.hetzner.com/cloud) - €5,49/Mo
- [Netcup VPS](https://www.netcup.com/de/server/vps) - €3,99/Mo
- [Contabo VPS](https://contabo.com/de/vps/) - €5,36/Mo

### Metadata-Services
- [TMDB](https://www.themoviedb.org) - Kostenlos
- [TVDB](https://www.thetvdb.com) - Kostenlos
- [RPDB](https://theratingdb.com) - Kostenlos bis Premium
- [MDBList](https://mdblist.com) - €1,20/Mo

### Tools
- [DuckDNS](https://www.duckdns.org) - Kostenlos
- [Caddy Server](https://caddyserver.com) - Kostenlos
- [Docker](https://www.docker.com) - Kostenlos

---