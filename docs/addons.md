# Anleitung für Stremio Addons

## AIOStreams
https://aiostreamsfortheweak.nhyira.dev/stremio/configure

### Services
- [TMDB](https://www.themoviedb.org/settings/api)
- [TVDB](https://www.thetvdb.com/api-information)
- RPDB (Free Tier: t0-free-rpdb)

### Addons
- Usenet Streamer: füge die Manifest URL ein, die zuvor in dem Webinterface des Usenet Streamer Addons angelegt wurde.

### Filters
- Resolution: 2160p, 1440p, 1080p, 720p
- Language: German
- Deduplicator: on

### Formatter 
[formatter](../configs/custom-formatter.json)

## AIOCatalogs
[AIOCatalogs](https://aio.pantelx.com/configure) ist ein Open-Source-Addon, das mehrere Katalog-Addons zu einem einzigen Addon kombiniert mit verbesserter Leistung und einer benutzerfreundlichen Konfigurationsoberfläche. Es verfügt über Multiplattform-Kompatibilität, serverlose Bereitstellungsoptionen und ein optimiertes Caching-System.

### Benötigte API Schlüssel
- [MDBList](https://mdblist.com/preferences/) ist ein Dienst, der personalisierte Film- und Serienlisten basierend auf Ihren Vorlieben und Bewertungen von verschiedenen Plattformen wie IMDb, Trakt und TMDb erstellt.
- RPDB (Free Tier: t0-free-rpdb): RPDB (Rating Poster Database) ist ein Dienst, der hochwertige Poster mit Bewertungen für Filme und Serien bereitstellt. Es hilft, die visuelle Darstellung in Stremio zu verbessern, indem es Poster mit Bewertungsinformationen anzeigt.

## AIOMetadata
https://aiometadatafortheweak.nhyira.dev/configure/

### Presets
Wähle ein Preset aus das am besten zu deinen Vorlieben passt.

### General
- Setze die Display Language auf German.
- Wenn nicht willst das Bilder einer Episode sichtbar sind (Spoilerschutz), aktiviere die Option "Hide Episode Spoilers".

### Integrations
- [TMDB](https://www.themoviedb.org/settings/api)
- [TVDB](https://www.thetvdb.com/api-information)
- RPDB (Free Tier: t0-free-rpdb)

### Catalog Management
Deaktiviere alle Kataloge, wir nutzen AIOCatalogs hierfür.

### Configuration
- Speichere die Konfiguration und sichere dir die UUID und das Passwort. 
- Installiere das Addon auf Stremio.